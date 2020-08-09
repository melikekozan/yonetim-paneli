<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      YÖNETTİĞİ E..
      <i style="float:right;" class="el-icon-circle-check"></i>
      <i style="float:right; margin-right:5px" class="el-icon-edit-outline"></i>
    </div>
    <div class="card-body">
      <fieldset class="user-border" style="position: relative">
        <legend class="user-border">ARA</legend>
        <el-input placeholder value></el-input>
        <i class="icon el-icon-search"></i>
      </fieldset>
      <fieldset class="user-border" style="position: relative">
        <legend class="user-border">EKRAN TÜRÜ</legend>
        <el-input placeholder value="İÇ ORTAM"></el-input>
        <i style="float:right; margin-left:5px" class="el-icon-house"></i>
        <i style=" float:right" class="el-icon-arrow-down"></i>
      </fieldset>
      <fieldset class="card-container">
        <legend class="user-border">8696435627593</legend>
        <div class="card-title">ŞEHİR MEYDANI</div>
        <div class="card-items">
          <div>
            <i class="el-icon-house"></i>İÇ ORTAM
          </div>
          <div>
            <i class="el-icon-refresh-right"></i>YATAY
          </div>
          <div>
            <i class="el-icon-wallet"></i>1920 X 1080 PİK
          </div>
        </div>
      </fieldset>
      <fieldset class="card-container">
        <legend class="user-border">8696435627593</legend>
        <div class="card-title">ŞEHİT SELİM AHISKALI PARKI</div>
        <div class="card-items">
          <div>
            <i class="el-icon-house"></i>İÇ ORTAM
          </div>
          <div>
            <i class="el-icon-refresh-right"></i>DİKEY
          </div>
          <div>
            <i class="el-icon-wallet"></i>256 X 768 PİK
          </div>
        </div>
      </fieldset>
      <fieldset class="card-container">
        <legend class="user-border">8696435627593</legend>
        <div class="card-title">MİLLİ MÜDAFA EĞİTİM VE KONGRE SALONU</div>
        <div class="card-items">
          <div>
            <i class="el-icon-cloudy"></i>DIŞ ORTAM
          </div>
          <div>
            <i class="el-icon-refresh-right"></i>DİKEY
          </div>
          <div>
            <i class="el-icon-wallet"></i>470 X 240 PİK
          </div>
        </div>
      </fieldset>
      <fieldset class="card-container">
        <legend class="user-border">8696435627593</legend>
        <div class="card-title">KÜTÜPHANE BEKLEME ODASI</div>
        <div class="card-items">
          <div>
            <i class="el-icon-cloudy"></i>DIŞ ORTAM
          </div>
          <div>
            <i class="el-icon-refresh-right"></i>KARE
          </div>
          <div>
            <i class="el-icon-wallet"></i>500 X 500 PİK
          </div>
        </div>
      </fieldset>
      <fieldset class="card-container">
        <legend class="user-border">8696435627593</legend>
        <div class="card-title">KÜTÜPHANE YEMEKHANE</div>
        <div class="card-items">
          <div>
            <i class="el-icon-cloudy"></i>DIŞ ORTAM
          </div>
          <div>
            <i class="el-icon-refresh-right"></i>YATAY
          </div>
          <div>
            <i class="el-icon-wallet"></i>1024 X 768 PİK
          </div>
        </div>
      </fieldset>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.card-container {
  display: flex;
  flex-direction: column;
  border: 1px solid black;
  border-radius: 12px;
  padding: 12px;
  margin: 5px 0px;
  position: relative;
}

.card-items {
  display: flex;
  width: 70px;
  justify-content: space-between;
  width: 80%;
  font-size: 10px;
}
.card {
  border-style: solid;
  border-color: #73c4be;
}
.card-header {
  color: #529991;
  background-color: #d2fafa;
  font-size: 14px;
  font-weight: bold;
  font-family: Verdana, Tahoma, sans-serif;
}
.card-header i {
  font-size: 17px;
}
.card-title {
  font-size: 11px;
}
</style>
