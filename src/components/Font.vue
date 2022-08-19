<template>
    <div class="bg">{{TextBackground}}</div>
    <div class="ft">{{TextFront}}</div>
</template>
<script lang="ts">
export default({
    name:"Font",
    props:["TextBackground","TextFront"],
})
</script>
<style>
.bg{
    font-size:70px;
    position:absolute;
    opacity:0.1;
    left:0;right:0;margin:0 auto;
    font-weight:bold;
    padding-top:20px
}
.ft{
    font-size: 60px; 
    font-weight:bold;
    padding-top: 50px;
    padding-bottom: 20px;
}
</style>