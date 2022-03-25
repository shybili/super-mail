<template>
    <div>
        <h2>我是demo组件</h2>
        <h2>{{msg}}</h2>
        <button @click="text">点击按钮</button>
    </div>
</template>
<script>
export default ({
    name:'demo',
    props:['msg'],
    setup(props,contexts) {
        console.log(props);

        function text(){
            contexts.emit('cw',8888);
        }

        return {
        text
        }
    },
   
})
</script>

<style >

</style>
