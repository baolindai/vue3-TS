<template>
<p>{{sum}}</p>
  
</template>

<script>
import { onMounted, reactive,toRefs } from 'vue'
import BigNumber  from "bignumber.js";
export default {
    name:"Home",
    setup(){
        const data=reactive({
            sum:null,
        })
        onMounted(()=>{
            let x = new BigNumber(0.3333);
            let sum=x.minus(0.2);
            data.sum=sum.valueOf()*1;
            console.log(typeof(data.sum),"sum")

        })
        return{
            ...toRefs(data)

        }

    }

}
</script>

<style>

</style>