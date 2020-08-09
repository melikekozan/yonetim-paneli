<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      BİLGİLERİ
      <i class="icn el-icon-circle-check"></i>
      <i style="margin-right:5px" class="icn el-icon-edit-outline"></i>
    </div>
    <div class="card-body">
      <div>
        <div class="container">
          <div class="profile-container">
            <fieldset class="card-border">
              <legend class="user-border">* ERKEK KULLANICI RESMİ</legend>
              <div class="icon-container">
                <i class="el-icon-s-custom large-icon"></i>
              </div>
            </fieldset>
          </div>
          <div class="profile-container">
            <fieldset class="card-border">
              <legend class="user-border">* KADIN KULLANICI RESMİ</legend>
              <div class="icon-container">
                <i class="el-icon-s-custom large-icon"></i>
              </div>
            </fieldset>
          </div>
        </div>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* AD SOYAD</legend>
          <el-input placeholder value="MACİT AHISKALI"></el-input>
          <i class="icon el-icon-user"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* BİRİM</legend>
          <el-input placeholder value="BASIN YAYIN"></el-input>
          <i class="icon el-icon-box"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* ÜNVAN</legend>
          <el-input placeholder value="MEMUR"></el-input>
          <i class="icon el-icon-price-tag"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">SABİT NUMARA</legend>
          <el-input placeholder value="0312 224 36 98 - 187"></el-input>
          <i class="icon el-icon-phone"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* CEP NUMARA</legend>
          <el-input placeholder value="0544 445 90 90"></el-input>
          <i class="iconn el-icon-mobile-phone"></i>
          <i class="icn el-icon-circle-plus-outline"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* E-POSTA</legend>
          <el-input placeholder value="macit.ahiskali@tika.gov.tr"></el-input>
          <i class="iconn el-icon-message"></i>
          <i class="icn el-icon-circle-plus-outline"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">ŞİFRE</legend>
          <el-input placeholder value="* * * * * * * * *"></el-input>
          <i class="iconn el-icon-key"></i>
          <i class="icn el-icon-view"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">* GİRİŞ DOĞRULAMA YÖNTEMİ</legend>
          <el-input placeholder value="SMS"></el-input>
          <i class="iconn el-icon-lock"></i>
          <i class="icn el-icon-arrow-down"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">İÇERİK ONAY YETKİSİ</legend>
          <el-input placeholder value="VERİLDİ"></el-input>
          <i class="iconn el-icon-circle-check"></i>
          <i class="icn el-icon-arrow-down"></i>
        </fieldset>
        <fieldset class="user-border" style="position: relative">
          <legend class="user-border">ERİŞİM IP ADRESİ</legend>
          <el-input placeholder value="192.168.2.259"></el-input>
          <i class="icn el-icon-location-outline"></i>
          <i class="icn el-icon-circle-plus-outline"></i>
          <i class="icn el-icon-search"></i>
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
.user-border {
  white-space: nowrap !important;
}
fieldset.user-border {
  border: 1px groove #73c4be !important;
  padding: 0 0.3em 0.3em 0.3em !important;
  margin: 0 0 0.5em 0 !important;
  -webkit-box-shadow: 0px 0px 0px 0px #73c4be;
  box-shadow: 0px 0px 0px 0px #73c4be;
}
.container {
  display: flex;
  justify-content: space-between;
  padding: 0 !important;
}
.profile-container {
  display: flex;
  border-radius: 5px !important;
  width: 48%;
  height: auto;
}
.profile-container i {
  font-size: 30px;
}

.card-border {
  border: 1px solid black;
  border-radius: 12px;
}
.icon {
  float: right;
  position: absolute;
  right: 5px;
  top: 30%;
  bottom: 30%;
}
.icon-container {
  width: 100%;
  text-align: center;
}

.large-icon {
  font-size: 96px !important;
  padding: 10px;
}

.iconn {
  float: right;
  margin-left: 5px;
}

.icn {
  float: right;
}
</style>