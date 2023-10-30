<template>

<button @click="show=!show">Click Me</button>    
<comp1 v-if="show"/>
</template>

<script>
import comp1 from '../components/comp1.vue';
export default{
    components:{comp1},

    data(){
        return{
            show:true
        }

    },
beforeUnmount(){
    console.log("before unmount")
},
Unmounted(){
    console.log("Unmounted")
}

}

</script>