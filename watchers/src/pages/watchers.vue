<template>
    GB:<input type="number" v-model.number="gb">
    MB:<input type="number" v-model.number="mb">
</template>

<script>
export default{
    data(){
        return{
            gb:null,
            mb:null,
         }
    },
    watch:{
        gb(value){
            this.mb=value*1024
        },
        mb(value){
            this.gb=value/1024
        }
    }
}
</script>