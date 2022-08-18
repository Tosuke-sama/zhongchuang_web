<template>
    <img :src="imgURL" alt="" style="width:100%;" >
</template>

<script lang="ts">
import { defineComponent, reactive } from 'vue';
export default defineComponent({
    name:'Header',
    setup(){
        const data = reactive({

        })
    },
    props:["imgURL"]//需要父组件照片的require函数路径
})
</script>