<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      KULLANICILAR
      <i style="float:right;" class="el-icon-circle-plus-outline"></i>
      <i style="float:right; margin-right:5px;" class="el-icon-delete"></i>
    </div>
    <div class="card-body">
      <fieldset class="user-border" style="position: relative">
        <legend class="user-border">ARA</legend>
        <el-input placeholder value></el-input>
        <i class="icon el-icon-search"></i>
      </fieldset>

      <fieldset class="user-border" style="position:relative;">
        <legend class="user-border">MÜDÜR</legend>
        <el-input placeholder="smth" value="SÜLEYMAN ALTINKAYA"></el-input>
      </fieldset>
      <fieldset class="user-border" style="position:relative;">
        <legend class="user-border">MEMUR</legend>
        <el-input placeholder="smth" value="TARIK SARI"></el-input>
      </fieldset>
      <fieldset class="user-border" style="position:relative;">
        <legend class="user-border">FOTOĞRAFÇI</legend>
        <el-input placeholder="smth" value="MACİT AHISKALI"></el-input>
      </fieldset>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: "",
    };
  },
};
</script>

<style>
.card {
  border-style: solid;
  border-color: #73c4be;
  border-width: 1.3px;
}
.card-header {
  color: #529991;
  background-color: #d2fafa;
  font-size: 14px;
  font-weight: bold;
  font-family: Verdana, Tahoma, sans-serif;
}
.card-body {
  padding: 10px;
}
.card-header i {
  font-size: 17px;
}
fieldset.user-border {
  border: 1px groove #73c4be !important;
  padding: 0 0.3em 0.3em 0.3em !important;
  margin: 0 0 0.5em 0 !important;
  -webkit-box-shadow: 0px 0px 0px 0px #73c4be;
  box-shadow: 0px 0px 0px 0px #73c4be;
  float: left;
  width: 100%;
  height: 40px;
}
legend.user-border {
  width: fit-content !important;
  background-color: unset;
  margin: 0 10px;
  padding: 0 6px;
  border-bottom: none !important;
  font-size: 9px;
  font-weight: bold;
  color: #3a4458;
}
div.el-input {
  height: 15px !important;
  position: absolute;
  top: 10px;
  left: -4px;
  padding: 0 !important;
  margin-left: 2px !important;
  font-size: 11px;
}
.icon {
  float: right;
  position: absolute;
  right: 5px;
  top: 30%;
  bottom: 30%;
}
.el-input__inner {
  border: 1px solid #fff !important;
  height: 20px !important;
  padding: 0 !important;
  margin: 0 8px;
  width: 80% !important;
}
</style>
