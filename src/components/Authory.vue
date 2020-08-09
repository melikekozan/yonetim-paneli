<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      YETKİLERİ
      <i style="float:right;" class="el-icon-circle-check"></i>
      <i style="float:right; margin-right:5px" class="el-icon-edit-outline"></i>
    </div>
    <div class="card-body">
      <el-collapse>
        <el-collapse-item class="custom-collapse">
          <template slot="title">
            <el-checkbox v-model="checkAll" @change="handleCheckAllChange">KULLANICI YÖNETİMİ</el-checkbox>
          </template>
          <hr />
          <el-checkbox-group v-model="checkedOptions" @change="handleCheckedOptions">
            <el-checkbox v-for="option in options" :label="option" :key="option">{{ option }}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
      <el-collapse>
        <el-collapse-item class="custom-collapse">
          <template slot="title">
            <el-checkbox
              v-model="checkAllSecreen"
              @change="handleCheckAllChangeScreen"
            >EKRAN YÖNETİMİ</el-checkbox>
          </template>
          <hr />
          <el-checkbox-group v-model="checkedScreens" @change="handleCheckedScreen">
            <el-checkbox v-for="screen in screens" :label="screen" :key="screen">{{ screen }}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
      <el-collapse>
        <el-collapse-item class="custom-collapse">
          <template slot="title">
            <el-checkbox
              v-model="checkAllContent"
              @change="handleCheckAllChangeContents"
            >İÇERİK YÖNETİMİ</el-checkbox>
          </template>
          <hr />
          <el-checkbox-group v-model="checkedContents" @change="handleCheckedContents">
            <el-checkbox v-for="content in contents" :label="content" :key="content">{{ content }}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
      <el-collapse>
        <el-collapse-item class="custom-collapse">
          <template slot="title">
            <el-checkbox
              v-model="checkAllSupport"
              @change="handleCheckAllChangeSupport"
            >DESTEK YÖNETİMİ</el-checkbox>
          </template>
          <hr />
          <el-checkbox-group v-model="checkedSupports" @change="handleCheckedSupports">
            <el-checkbox v-for="support in supports" :label="support" :key="support">{{ support }}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
      <el-collapse>
        <el-collapse-item class="custom-collapse">
          <template slot="title">
            <el-checkbox
              v-model="checkAllClient"
              @change="handleCheckAllChangeClients"
            >MÜŞTERİ YÖNETİMİ</el-checkbox>
          </template>
          <hr />
          <el-checkbox-group v-model="checkedClients" @change="handleCheckedClients">
            <el-checkbox v-for="client in clients" :label="client" :key="client">{{ client }}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
    </div>
  </div>
</template>

<script>
const Options = ["GÖRÜNTÜLEME", "EKLEME", "DÜZENLEME", "SİLME"];
const Screens = [
  "GÖRÜNTÜLEME",
  "EKLEME",
  "DÜZENLEME",
  "SİLME",
  "E-POSTA BİLDİRİMİ",
  "SMS BİLDİRİMİ",
];
const Supports = [
  "DESTEK TALEBİ OLUŞTURMA",
  "YANITLAMA",
  "GÖRÜNTÜLEME",
  "SİLME",
  "E-POSTA BİLDİRİMİ",
  "SMS BİLDİRİMİ",
];
const Contents = [
  "GÖRÜNTÜLEME",
  "EKLEME",
  "DÜZENLEME",
  "SİLME",
  "E-POSTA BİLDİRİMİ",
  "SMS BİLDİRİMİ",
];
const Clients = ["X", "Y", "Z"];

export default {
  data() {
    return {
      checkAll: false,
      checkAllSecreen: false,
      checkAllSupport: false,
      checkAllContent: false,
      checkAllClient: false,
      checkedOptions: [],
      options: Options,
      checkedScreens: [],
      screens: Screens,
      checkedSupports: [],
      supports: Supports,
      checkedContents: [],
      contents: Contents,
      checkedClients: [],
      clients: Clients,
    };
  },
  methods: {
    handleCheckAllChange(val1) {
      this.checkedOptions = val1 ? Options : [];
      this.isIndeterminate = false;
    },
    handleCheckedOptions(value1) {
      let checkedCount = value1.length;
      this.checkAll = checkedCount === this.options.length;
      this.isIndeterminate =
        checkedCount > 0 && checkedCount < this.options.length;
    },
    handleCheckAllChangeScreen(val2) {
      this.checkedScreens = val2 ? Screens : [];
      this.isIndeterminate = false;
    },
    handleCheckedScreen(value2) {
      let checkedCount1 = value2.length;
      this.checkAllSecreen = checkedCount1 === this.screens.length;
      this.isIndeterminate =
        checkedCount1 > 0 && checkedCount1 < this.screens.length;
    },
    handleCheckAllChangeSupport(val3) {
      this.checkedSupports = val3 ? Supports : [];
      this.isIndeterminate = false;
    },
    handleCheckedSupports(value3) {
      let checkedCount2 = value3.length;
      this.checkAllSupport = checkedCount2 === this.supports.length;
      this.isIndeterminate =
        checkedCount2 > 0 && checkedCount2 < this.supports.length;
    },
    handleCheckAllChangeContents(val4) {
      this.checkedContents = val4 ? Contents : [];
      this.isIndeterminate = false;
    },
    handleCheckedContents(value4) {
      let checkedCount3 = value4.length;
      this.checkAllContent = checkedCount3 === this.contents.length;
      this.isIndeterminate =
        checkedCount3 > 0 && checkedCount3 < this.contents.length;
    },
    handleCheckAllChangeClients(val5) {
      this.checkedClients = val5 ? Clients : [];
      this.isIndeterminate = false;
    },
    handleCheckedClients(value5) {
      let checkedCount4 = value5.length;
      this.checkAllClient = checkedCount4 === this.clients.length;
      this.isIndeterminate =
        checkedCount4 > 0 && checkedCount4 < this.clients.length;
    },
  },
};
</script>

<style>
.card {
  margin-right: 8px;
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

.el-checkbox-group {
  display: flex !important;
  flex-direction: column;
}

.el-checkbox__label {
  font-size: 11px !important;
}
.el-checkbox__input.is-checked .el-checkbox__inner,
.el-checkbox__input.is-indeterminate .el-checkbox__inner {
  background-color: #3a4458 !important;
  border-color: #3a4458 !important;
}
</style>
