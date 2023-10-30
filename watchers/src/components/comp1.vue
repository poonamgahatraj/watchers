<template>
<h1 ref="comp">Before Unmount and Unmounted</h1>

</template>
<script>
export default{
    beforeUnmount(){
    console.log("before unmount",this.$refs['comp'])
},
   unmounted(){
    console.log("Unmounted" ,this.$refs['comp'])
}
}
</script>