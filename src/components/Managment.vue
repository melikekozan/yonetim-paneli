<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      YÖNETTİĞİ E..
      <i style="float:right;" class="el-icon-circle-check"></i>
      <i style="float:right; margin-right:5px" class="el-icon-edit-outline"></i>
    </div>
    <div class="card-container">
      <div class="card-title">title</div>
      <div class="card-items">
        <div>1</div>
        <div>2</div>
        <div>3</div>
      </div>
    </div>
    <div>card 1</div>
    <div>card 1</div>
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
  margin: 5px 10px
}

.card-items {
  display: flex;
  width: 70px;
  justify-content: space-between;
  width: 80% 
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
</style>
