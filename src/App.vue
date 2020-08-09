<template>
  <div id="app">
    <Header></Header>
    <el-row>
      <el-col :span="1">
        <Navbar></Navbar>
      </el-col>
      <el-col :span="23">
        <div class="main">
          <el-row>
            <el-col :span="6">
              <Clients></Clients>
            </el-col>
            <el-col :span="6">
              <Informations></Informations>
            </el-col>
            <el-col :span="6">
              <Authory></Authory>
            </el-col>
            <el-col :span="6">
              <Managment></Managment>
            </el-col>
          </el-row>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Header from "./components/Header";
import Authory from "./components/Authory";
import Clients from "./components/Clients";
import Informations from "./components/Informations";
import Managment from "./components/Managment";
import Navbar from "./components/Navbar";

export default {
  name: "app",
  components: {
    Header,
    Authory,
    Clients,
    Informations,
    Managment,
    Navbar,
  },
};
</script>

<style>
#app {
  background-color: #eeeff9;
}
.main {
  margin-top: 10px;
  margin-left: 7px;
}
</style>
