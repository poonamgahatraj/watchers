<template>
    <h1>Hello</h1>
    <h2>Good morning</h2>
</template>

<script>
export default{


    //beforeCreate(){
    //    alert ("before create")
    //},

    //created(){
     //   alert("component created")
    //}

    beforeMount(){
        console.log("beforemount", this.$el)
    },

    mounted(){
        console.log("mounted",this.$el)
    }

}
</script>

<style>
h1{
    color:red;
}
</style>