<template>
    <button @click="click"  :style="styles" :disabled="disabled" :class="disabled?'dse-button disable':'dse-button enable'">
        {{disabled?disablecontent:enablecontent}}
    </button>
</template>
<script>
    export default {
        name:'DButton',
        props:{
            enablecontent:{
                type:String,
                default:"操作"
            },
            styles:{
                type:String,
                default:null
            },
            disablecontent:{
                type:String,
                default:"操作中..."
            },
            click:{
                type:Function,
                default:null
            },
            disabled:{
                type:Boolean,
                default:false
            }  
        }
    }
</script>
<style scoped lang="less">
    .dse-button{
        padding:2px 5px;
        color: #fff;
        text-align: center;
        border-radius: 3px;
        border: none;
        outline: none;
    }
    .enable{
        background-color: #0085ff;
    }
    .disable{
        background-color: #ddd;
    }
</style>
