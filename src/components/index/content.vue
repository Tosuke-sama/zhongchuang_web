<template>
  <el-row style="padding-bottom:50px">
    <el-col
      v-for="(o, index) in 3"
      :key="o"
      :span="5"
      :offset="index > 0 ? 0.5 : 0"
      :push="4"
      class="card"
    >
      <el-card :body-style="{ padding: '10px' } " shadow="hover">
        <img
          src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png"
          class="image"
        />
        <div style="padding: 50px">
          <span>对于企业或者公司来说，基于成本控制是不可避免的</span>
        </div>
      </el-card>
    </el-col>
  </el-row>
</template>

<script lang="ts">
export default({
    name:"content",
})
</script>

<style scoped>
.time {
  font-size: 12px;
  color: #999;
}
.image {
  width: 100%;
  display: block;
}
.card{
  width: 70%;
 display: flex;
 flex-direction: column;
}
.el-card__body{
    height: 50%;
    width: 33%;
}
.box-card{
        /* position: absolute; */
        top: 0;
        left: 0;
        right:0;
        bottom: 0;
        margin: auto;
    }
</style>

