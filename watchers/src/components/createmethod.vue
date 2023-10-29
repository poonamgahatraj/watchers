<template>
    <h1>Hello</h1>
    <h2>Good morning</h2>
    <h1 ref="count">{{ count }}</h1>
    <button @click="count=count+1">update button</button>
</template>

<script>
export default{

    data(){
        return{
            count:0
        }
    },


    //beforeCreate(){
    //    alert ("before create")
    //},

    //created(){
     //   alert("component created")
    //}

    //beforeMount(){
      //  console.log("beforemount", this.$el)
    //},

    //mounted(){
      //  console.log("mounted",this.$el)
    //}

    beforeUpdate(){
        console.log("before update", this.$refs['count'].textContent)
    },

    updated(){
        console.log("update", this.$refs['count'].textContent)
    }

}
</script>

<style>
h1{
    color:red;
}
</style>