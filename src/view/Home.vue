<template>
  <div class="container">
    <div
      class="left"
      style="background-color: white; width: 60%; height: 99%; margin: 5px; border-radius: 5px;"
    >
      <!-- 左上角店板块 -->
      <div class="box top-left">
        <img
          src="../assets/img/store.png"
          width="30px"
          height="30px"
        >
        <span style=" font-size: 20px; font-weight: 700;">店</span>
        <span style="font-size: 12px; font-weight: 700; position: absolute; top: 25px; left: 75px;">
          -选择门店，圈定人货范围，按店开展营销
        </span>

        <img
          src="../assets/img/place.png"
          width="25px"
          height="25px"
          style="position: absolute; left: 530px;"
        >
        <span style="position: absolute;  font-size: 14px;  left: 555px; top: 24px;">主要地区：广州</span>

        <div
          class="top-left-button1"
          @click="onClickOutside()"
        >
          <span style="font-size: 12px;">圈选店人货</span>
          <img
            src="../assets/img/icon1.png"
            width="12px"
            height="12px"
          >
        </div>
        <div class="top-left-item1">
          <span style="color: gray; font-size: 13px;">已选门店</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">23</span>
        </div>
        <div class="top-left-item2">
          <span style="color: gray; font-size: 13px;">活跃会员数</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">232,300</span>
        </div>
        <div class="top-left-item3">
          <span style="color: gray; font-size: 13px;">平均月销售额</span>
          <div class="top-left-item3-item">
            <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">￥</span>
            <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">222,423</span>
          </div>
        </div>
        <div class="top-left-item4">
          <span style="color: gray; font-size: 13px;">平均售罄率</span>
          <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">45%</span>
        </div>
        <div class="top-left-item5">
          <span style="color: gray; font-size: 13px;">客单价</span>
          <div class="top-left-item5-item">
            <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">￥</span>
            <span style="font-size: 20px; margin-top: 10px; font-weight: 700;">34,544</span>
          </div>
        </div>
        <button class="top-left-button2">导入门店</button>
      </div>
      <!-- 左下角人和货板块 -->
      <div class="box bottom-left">
        <!-- 左边板块 -->
        <div class="bottom-left-block1">
          <Goods v-if="!isClick"></Goods>
          <Person v-if="isClick"></Person>
        </div>
        <!-- 右边板块 -->
        <div class="bottom-left-block2">
          <Goods v-if="isClick"></Goods>
          <Person v-if="!isClick"></Person>
        </div>
        <img
          src="../assets/img/change.png"
          width="35px"
          height="35px"
          style="position: absolute; top: 20%;left: 47%;cursor: pointer;"
          @click="Change()"
        >
        <div class="line"></div>
      </div>
    </div>

    <div class="box top-right">
      <Ai v-if="isActive3"></Ai>
    </div>
    <div class="box bottom-right">
      <Sales v-if="isActive4"></Sales>
    </div>

  </div>
  <!-- 匹配按钮 -->
  <button
    class="button1"
    :class="{ active: isActive,active2: isActive2}"
    @click="btnActive()"
  >
    <span class="btn-span">匹配</span>
    <img
      src="../assets/img/ai.png"
      class="btn-icon1"
    >
    <img
      src="../assets/img/icon4.png"
      class="btn-icon2"
    >
  </button>
</template>
<script setup>
import Goods from "../components/Goods.vue";
import Person from "../components/Person.vue";
import Ai from "../components/Ai.vue";
import Sales from "../components/Sales.vue";
import { ref } from "vue";

const isClick = ref(false); //是否点击切换按钮
const isActive = ref(false); //为匹配按钮添加active类
const isActive2 = ref(false); //为匹配按钮添加active2类
// 让右边两个板块分别延时出现
const isActive3 = ref(false);
const isActive4 = ref(false);

// 匹配按钮点击事件
const btnActive = () => {
  setTimeout(() => {
    isActive.value = true;
    setTimeout(() => {
      isActive2.value = true;
      setTimeout(() => {
        isActive3.value = true;
        setTimeout(() => {
          isActive4.value = true;
        }, 300);
      }, 300);
    }, 300);
  }, 300);
};
// 人货两个板块左右切换
const Change = () => {
  isClick.value = !isClick.value;
};
</script>
  <style scoped>
.container {
  position: relative;
  width: 1500px;
  height: 770px;
  overflow: hidden;
  background: rgba(188, 215, 243, 0.9);
}

.box {
  position: absolute;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  opacity: 1;
  border-radius: 8px;
  background: rgba(252, 253, 255, 1);
  border: 1px solid rgba(189, 209, 255, 1);
}

.top-left {
  width: 58%;
  height: 23%;
  top: 10px;
  left: 10px;
}
.top-right {
  width: 38%;
  height: 38%;
  top: 10px;
  right: 10px;
}
.bottom-left {
  width: 58%;
  height: 73%;
  bottom: 10px;
  left: 10px;
}
.bottom-right {
  width: 38%;
  height: 58%;
  bottom: 10px;
  right: 10px;
}
.top-left-button1 {
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 90px;
  height: 20px;
  padding: 4px;
  position: absolute;
  cursor: pointer;
  top: 0px;
  right: 0px;
  opacity: 1;
  border-radius: 0px 8px 0px 16px;
  background: rgba(112, 135, 250, 1);
}
.top-left-item1 {
  position: absolute;
  bottom: 40px;
  left: 40px;
}
.top-left-item1 span {
  display: block;
  text-align: center;
}
.top-left-item2 {
  position: absolute;
  bottom: 40px;
  left: 160px;
}
.top-left-item2 span {
  display: block;
  text-align: center;
}
.top-left-item3 {
  position: absolute;
  bottom: 40px;
  left: 290px;
  display: block;
  text-align: center;
}
.top-left-item3-item {
  display: flex;
  align-items: center;
}
.top-left-item4 {
  position: absolute;
  bottom: 40px;
  left: 440px;
}
.top-left-item4 span {
  display: block;
  text-align: center;
}
.top-left-item5 {
  position: absolute;
  bottom: 40px;
  left: 550px;
  display: block;
  text-align: center;
}
.top-left-item5-item {
  display: flex;
  align-items: center;
}
.top-left-button2 {
  width: 70px;
  height: 20px;
  position: absolute;
  right: 30px;
  bottom: 70px;
  border: 1px solid rgba(252, 151, 73, 1);
  border-radius: 10px;
  background-color: rgba(255, 248, 242, 1);
  color: rgba(252, 151, 73, 1);
  cursor: pointer;
  font-size: 12px;
}
.bottom-left {
  display: flex;
  justify-content: space-between;
}
.bottom-left-block1,
.bottom-left-block2 {
  flex: 1;
  margin: 0 10px;
}
.line {
  position: absolute;
  left: 415px;
  top: 30%;
  width: 1px;
  height: 350px;
  border-left: 2px dashed #ccc;
  margin: 0 10px;
}
.button1 {
  position: absolute;
  left: 850px;
  top: 150px;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: none;
  cursor: pointer;
  background: linear-gradient(
    208.59deg,
    rgba(253, 150, 74, 1) 0%,
    rgba(255, 231, 181, 1) 100%
  );
  border: 0px;
  font-size: 24px;
  font-weight: 600;
  box-shadow: 0 8px 16px rgba(253, 150, 74, 0.3);
  transition: all 0.3s ease;
}
.btn-text {
  opacity: 1;
}
.btn-icon1 {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
  width: 70%;
  transition: opacity 0.3s ease, filter 0.3s ease;
}
.btn-icon2 {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
  width: 20%;
  transition: opacity 0.3s ease, filter 0.3s ease;
}
.button1.active {
  background: rgba(255, 242, 217, 1);
  border: 1px solid rgba(254, 177, 109, 1);
}
.button1.active .btn-span {
  opacity: 0;
}
.button1.active .btn-icon1 {
  opacity: 1;
}
.button1.active.active2 {
  background: linear-gradient(
    208.59deg,
    rgba(253, 150, 74, 1) 0%,
    rgba(255, 231, 181, 1) 100%
  );
  border: 0px;
}
.button1.active.active2 .btn-span {
  opacity: 0;
}
.button1.active.active2 .btn-icon1 {
  opacity: 0;
}
.button1.active.active2 .btn-icon2 {
  opacity: 1;
}
</style>