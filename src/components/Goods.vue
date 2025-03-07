<template>
  <div class="Goods">
    <img
      src="../assets/img/goods.png"
      width="30px"
      height="30px"
    >
    <span style=" font-size: 20px; font-weight: 700; margin-left: 5px;">货</span>
    <span style="font-size: 12px; font-weight: 700; position: absolute; top: 8px; left: 60px;">
      -限定卖货范围
    </span>

    <span style="position: absolute; left: 130px; top: 70px; font-weight: 700;">选择商品分组</span>
    <button class="button1">2023年春夏款库存充足 ></button>
    <img
      src="../assets/img/icon2.png"
      width="20px"
      height="10px"
      style="position: absolute; left: 160px; top: 180px; opacity: 0.5;"
    >
    <img
      src="../assets/img/icon2.png"
      width="20px"
      height="10px"
      style="position: absolute; left: 160px; top: 190px;"
    >
    <div class="item1">
      <span style="color: gray; font-size: 13px;">款数</span>
      <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">834</span>
    </div>
    <div class="item2">
      <span style="color: gray; font-size: 13px;">库存</span>
      <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">29,234</span>
    </div>
    <div class="item3">
      <span style="color: gray; font-size: 13px;">库龄</span>
      <div class="item3-item">
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">3</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">年</span>
      </div>
    </div>
    <div class="item4">
      <span style="color: gray; font-size: 13px;">售罄率</span>
      <div class="item4-item">
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">3</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">%</span>
      </div>
    </div>
    <div class="item5">
      <span style="color: gray; font-size: 13px;">主要商品</span>
      <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">T恤</span>
    </div>
    <div class="item6">
      <span style="color: gray; font-size: 13px;">价格带</span>
      <div class="item6-item">
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">￥</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">1,000-3,000</span>
      </div>
    </div>
    <div class="item7">
      <span style="color: gray; font-size: 13px;">折扣率</span>
      <div class="item7-item">
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">56</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">%</span>
      </div>
    </div>
    <div class="item8">
      <span style="color: gray; font-size: 13px;">销售状态</span>
      <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">畅销</span>
    </div>
    <button class="button2">商品明细</button>
  </div>
</template>
<style scoped>
.Goods {
  width: 380px;
  height: 520px;
  position: absolute;
  display: flex;
}
.button1 {
  width: 160px;
  height: 25px;
  font-size: 12px;
  position: absolute;
  left: 100px;
  top: 120px;
  background-color: white;
  border: 1px solid gray;
  border-radius: 5px;
  cursor: pointer;
}
.item1 {
  position: absolute;
  bottom: 240px;
  left: 10px;
}
.item1 span {
  display: block;
  text-align: center;
}
.item2 {
  position: absolute;
  bottom: 240px;
  left: 110px;
}
.item2 span {
  display: block;
  text-align: center;
}
.item3 {
  position: absolute;
  bottom: 240px;
  left: 240px;
  display: block;
  text-align: center;
}
.item3-item {
  display: flex;
  align-items: center;
}
.item4 {
  position: absolute;
  bottom: 240px;
  left: 310px;
  display: block;
  text-align: center;
}
.item4-item {
  display: flex;
  align-items: center;
}
.item5 {
  position: absolute;
  bottom: 120px;
  left: 0px;
}
.item5 span {
  display: block;
  text-align: center;
}
.item6 {
  position: absolute;
  bottom: 120px;
  left: 70px;
  display: block;
  text-align: center;
}
.item6-item {
  display: flex;
  align-items: center;
}
.item7 {
  position: absolute;
  bottom: 120px;
  left: 240px;
  display: block;
  text-align: center;
}
.item7-item {
  display: flex;
  align-items: center;
}
.item8 {
  position: absolute;
  bottom: 120px;
  left: 310px;
}
.item8 span {
  display: block;
  text-align: center;
}
.button2 {
  width: 80px;
  height: 30px;
  font-size: 12px;
  position: absolute;
  left: 140px;
  bottom: 40px;
  background-color: rgba(252, 151, 73, 1);
  border-radius: 20px;
  border: 0;
  color: white;
  cursor: pointer;
}
</style>