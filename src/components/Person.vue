<template>
  <div class="Person">
    <img
      src="../assets/img/goods.png"
      width="30px"
      height="30px"
    >
    <span style=" font-size: 20px; font-weight: 700; margin-left: 5px;">人</span>
    <span style="font-size: 12px; font-weight: 700; position: absolute; top: 8px; left: 60px;">
      -明确营销对象
    </span>
    <div
      class="isPerson"
      v-if="isSelect === 'People'"
    >

      <span style="position: absolute; left: 130px; top: 70px; font-weight: 700;">选择会员分组</span>
      <button class="button1">2月正价核心会员群 ></button>
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
        <span style="color: gray; font-size: 13px;">分组会员</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">9,213</span>
      </div>
      <div class="item2">
        <span style="color: gray; font-size: 13px;">开卡率</span>
        <div class="item2-item">
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">34</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">%</span>
        </div>
      </div>
      <div class="item3">
        <span style="color: gray; font-size: 13px;">主类型</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">老会员</span>
      </div>
      <div class="item4">
        <span style="color: gray; font-size: 13px;">年龄段</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">30-50</span>
      </div>
      <div class="item5">
        <span style="color: gray; font-size: 13px;">复购率</span>
        <div class="item5-item">
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">12</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">%</span>
        </div>
      </div>
      <div class="item6">
        <span style="color: gray; font-size: 13px;">RFM</span>
        <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">重要发展</span>
      </div>
      <div class="item7">
        <span style="color: gray; font-size: 13px;">平均折扣</span>
        <div class="item7-item">
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">87</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">%</span>
        </div>
      </div>
      <div class="item8">
        <span style="color: gray; font-size: 13px;">客单价</span>
        <div class="item8-item">
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">￥</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">1213.9</span>
        </div>
      </div>
      <button class="button2">指标洞察</button>
      <button class="button3">会员分析</button>
    </div>
    <div
      class="isAI"
      v-if="isSelect === 'Ai'"
    >
      <img
        src="../assets/img/plan.png"
        width="200px"
        height="200px"
        style="position: absolute; top: 150px;left: 100px;"
      >
      <span style="position: absolute;  top: 350px;left: 90px;">点击右方匹配按钮，立即生成方案~</span>
    </div>
    <div class="radio">
      <input
        type="radio"
        id="ai"
        v-model="isSelect"
        value="Ai"
      />
      <label for="ai">Ai选</label>
      <input
        type="radio"
        id="people"
        v-model="isSelect"
        value="People"
        checked
      >
      <label for="people">自选</label>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";

const isSelect = ref("People");
</script>
  <style scoped>
.Person {
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
  display: block;
  text-align: center;
}
.item2-item {
  display: flex;
  align-items: center;
}
.item3 {
  position: absolute;
  bottom: 240px;
  left: 200px;
}
.item3 span {
  display: block;
  text-align: center;
}
.item4 {
  position: absolute;
  bottom: 240px;
  left: 310px;
}
.item4 span {
  display: block;
  text-align: center;
}
.item5 {
  position: absolute;
  bottom: 120px;
  left: 10px;
  display: block;
  text-align: center;
}
.item5-item {
  display: flex;
  align-items: center;
}
.item6 {
  position: absolute;
  bottom: 120px;
  left: 90px;
}
.item6 span {
  display: block;
  text-align: center;
}
.item7 {
  position: absolute;
  bottom: 120px;
  left: 210px;
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
  left: 295px;
  display: block;
  text-align: center;
}
.item8-item {
  display: flex;
  align-items: center;
}
.button2 {
  width: 80px;
  height: 30px;
  font-size: 12px;
  position: absolute;
  left: 80px;
  bottom: 40px;
  background-color: rgba(37, 207, 130, 1);
  border-radius: 20px;
  border: 0;
  color: white;
  cursor: pointer;
}
.button3 {
  width: 80px;
  height: 30px;
  font-size: 12px;
  position: absolute;
  left: 200px;
  bottom: 40px;
  background-color: rgba(252, 151, 73, 1);
  border-radius: 20px;
  border: 0;
  color: white;
  cursor: pointer;
}
.radio {
  position: absolute;
  left: 320px;
  top: 50px;
}
input[type="radio"],
input[type="radio"] + label {
  cursor: pointer;
}
input[type="radio"]:checked + label {
  color: rgb(55, 222, 55);
  font-weight: 500;
  text-decoration: underline;
}
</style>