<template>
    <demo  @cw="says" msg="你好啊"></demo>
   
</template>
<script>
import demo from './components/demo.vue'
export default ({
    name:'App',
    components:{
       demo 
    },
    setup() {
        function says(value){
            alert(`你好啊，我的大哥${value}`)
        }


        return {
        says
        }
    },
    
})
</script>

<style >

</style>
