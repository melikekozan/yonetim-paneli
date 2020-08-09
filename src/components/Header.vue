<template>
  <el-menu
    :default-active="activeIndex2"
    class="el-menu-demo"
    mode="horizontal"
    @select="handleSelect"
    background-color="#28323C"
    text-color="#70767B"
    active-text-color="#fff"
  >
    <el-menu-item style="color:#fff;">
      <a style="text-decoration:none;" href="https://www.duyurubu.com/">DUYURUBU</a>
    </el-menu-item>
    <el-menu-item index="2" style="color:#9eeeec">
      <i style="color:#70767B" class="el-icon-house"></i>
    </el-menu-item>

    <el-menu-item index="3" style>
      <i style="color:#70767B" class="el-icon-message-solid"></i>
    </el-menu-item>
    <el-menu-item index="4" style="color:#9eeeec">
      <i style="color:#70767B" class="el-icon-full-screen"></i>
    </el-menu-item>
    <el-menu-item style="float:right; padding:0 10px">
      <el-dropdown>
        <el-button style="background-color: #28323C">
          <span class="el-dropdown-link">
            Macit AHISKALI
            <i class="el-icon-arrow-down el-icon--right"></i>
          </span>
        </el-button>
        <el-dropdown-menu slot="dropdown">
          <el-dropdown-item>
            <i class="el-icon-user"></i>KULLANICI AYARLARI
          </el-dropdown-item>
          <el-dropdown-item>
            <i class="el-icon-setting"></i>DÜZEN AYARLARI
          </el-dropdown-item>
          <el-dropdown-item>
            <i class="el-icon-circle-close"></i>ÇIKIŞ YAP
          </el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown>
    </el-menu-item>
    <el-menu-item style="float:right;  padding:0 0px">
      <div class="demo-basic--circle">
        <div class="block" size="small">
          <el-avatar shape="square" :src="squareUrl"></el-avatar>
        </div>
      </div>
    </el-menu-item>
    <p id="text" style>Yönetim Sayfasına Hoş Geldiniz</p>
  </el-menu>
</template>


<script>
export default {
  data() {
    return {
      activeIndex: "1",
      activeIndex2: "1",
      squareUrl:
        "https://cube.elemecdn.com/9/c2/f0ee8a3c7c9638a54940382568c9dpng.png",
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style>
.el-menu.el-menu--horizontal {
  border-bottom: solid 3px #73c4be !important;
}
li.el-menu-item {
  height: 40px;
  font-size: 17px;
  padding: 0 10px;
}
#text {
  color: #fff;
  float: right;
  font-size: 12px;
  padding: 0 13px;
  margin-top: 25px;
}
.el-dropdown-link {
  cursor: pointer;
  color: #fff;
}
.el-icon-arrow-down {
  font-size: 12px;
}
.el-dropdown-menu__item:focus,
.el-dropdown-menu__item:not(.is-disabled):hover {
  color: #529991 !important;
}
</style>