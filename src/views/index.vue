<template>
      <div class="common-layout">
    <el-container>
      <el-header> <Header/> </el-header>
      <el-main>Main</el-main>
      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>
<script lang="ts">
import Header from'@/components/Header.vue'
import { defineComponent } from 'vue';
export default{
    name:'index',
    components:{
        Header,
    }
}
</script>