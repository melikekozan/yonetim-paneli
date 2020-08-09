<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      BİLGİLERİ
      <i style="float:right;" class="el-icon-circle-check"></i>
      <i style="float:right; margin-right:5px" class="el-icon-edit-outline"></i>
    </div>
    <div class="card-body">
      <div>
        <div class="container">
          <div class="profile-container">
            <fieldset class="user-border">
              <legend class="user-border">* ERKEK KULLANICI RESMİ</legend>
              <div class="control"></div>
              <label style="font-size:11px; padding:0 0 0 5px;"></label>
              <i class="el-icon-s-custom"></i>
            </fieldset>
          </div>
          <div class="profile-container">
            <fieldset class="user-border">
              <legend class="user-border">* KADIN KULLANICI RESMİ</legend>
              <div class="control"></div>
              <label style="font-size:11px; padding:0 0 0 5px;"></label>
              <i class="el-icon-s-custom"></i>
            </fieldset>
          </div>
        </div>
        <fieldset class="user-border">
          <legend class="user-border">* AD SOYAD</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* BİRİM</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* ÜNVAN</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* SABİT NUMARA</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* CEP NUMARA</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* E-POSTA</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* ŞİFRE</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* GİRİŞ DOĞRULAMA YÖNTEMİ</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* AD SOYAD</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border">
          <legend class="user-border">* AD SOYAD</legend>
          <div class="control"></div>
          <label style="font-size:11px; padding:0 0 0 5px;">MACİT AHISKALI</label>
          <i style="float:right; margin-right:5px" class="el-icon-user"></i>
        </fieldset>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
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
  height: calc(100vh - 40px);
  width: 100% !important;
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
}
legend.user-border {
  width: inherit;
  padding: 0 10px;
  border-bottom: none;
  font-size: 9px;
  font-weight: bold;
  color: #3a4458;
}
.container {
}
.profile-container {
  display: flex;
  border-radius: 5px !important;
  width: 130px;
  height: auto;
}
.profile-container i {
  font-size: 30px;
  position: absolute;
  padding: 0 0 0 30px;
}
</style>