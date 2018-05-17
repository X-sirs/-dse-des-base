<template>
    <div @click="click" class="dse-button">
        按钮
    </div>
</template>
<script>
    export default {
        name:'button',
        methods:{
            click(){
                console.log("test package")
            }
        }
    }
</script>
<style scoped lang="less">
    .dse-button{
        background-color: #0085ff;
    }
</style>
