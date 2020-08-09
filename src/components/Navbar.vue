<template>
  <el-row class="tac">
    <el-col>
      <el-menu
        id="aaa"
        default-active="2"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
        background-color="#3C465A"
        text-color="#70767B"
        active-text-color="#fff"
      >
        <el-menu-item index="1">
          <i class="el-icon-user"></i>
        </el-menu-item>
        <el-menu-item index="2">
          <i class="el-icon-monitor"></i>
        </el-menu-item>
        <el-menu-item index="3">
          <i class="el-icon-video-play"></i>
        </el-menu-item>
        <el-menu-item index="4">
          <i class="el-icon-setting"></i>
        </el-menu-item>
        <el-menu-item index="5">
          <i class="el-icon-service"></i>
        </el-menu-item>
      </el-menu>
    </el-col>
  </el-row>
</template>


<script>
export default {
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style>
#aaa {
  height: calc(100vh - 63px);
  width: 100% !important;
  padding: 0;
  margin: 0;
}
#aaa:last-child {
  margin-top: auto;
}
li.el-menu-item {
  height: 50px;
  padding: -1 10px !important;
}
</style>