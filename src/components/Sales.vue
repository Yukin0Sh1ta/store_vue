<template>
  <div class="sale">
    <div class="chang">
      <div class="title">
        <span style="font-size: 12px;">按店推荐</span>
      </div>
      <img
        src="../assets/img/icon6.png"
        width="30px"
        height="30px"
        style="margin: 3px;"
      >
      <span style=" font-size: 20px; font-weight: 700; margin: 3px;">场</span>
      <span style="font-size: 12px; font-weight: 700; position: absolute; top: 5px; left: 60px;margin: 3px;">
        -营销活动配置
      </span>

      <div class="btn_group">
        <div class="button1">活动</div>
        <div class="button2">互动</div>
        <div class="button3">内容</div>
      </div>

      <div class="item1">
        <img
          src="../assets/img/sale_icon1.png"
          width="45px"
          height="40px"
        >
        <span>权益</span>
      </div>
      <div class="item2">
        <img
          src="../assets/img/sale_icon2.png"
          width="45px"
          height="40px"
        >
        <span>优惠券</span>
      </div>
      <div class="item3">
        <img
          src="../assets/img/sale_icon3.png"
          width="45px"
          height="40px"
        >
        <span>促销</span>
      </div>
      <div class="item4">
        <img
          src="../assets/img/sale_icon4.png"
          width="45px"
          height="40px"
        >
        <span>常态化</span>
      </div>
      <div class="item5">
        <img
          src="../assets/img/sale_icon5.png"
          width="45px"
          height="40px"
        >
        <span>引流到店</span>
      </div>
    </div>
    <div class="chuda">
      <img
        src="../assets/img/icon7.png"
        width="30px"
        height="30px"
        style="margin: 3px;"
      >
      <span style=" font-size: 20px; font-weight: 700; margin: 3px;">触达</span>
      <span style="font-size: 12px; font-weight: 700; position: absolute; top: 5px; left: 80px;margin: 3px;">
        -多点触达提高转化率
      </span>

      <div class="item6">
        <img
          src="../assets/img/sale_icon6.png"
          width="45px"
          height="40px"
        >
        <span>导购任务</span>
      </div>
      <div class="item7">
        <img
          src="../assets/img/sale_icon7.png"
          width="45px"
          height="40px"
        >
        <span>企微群发</span>
      </div>
      <div class="item8">
        <img
          src="../assets/img/sale_icon8.png"
          width="45px"
          height="40px"
        >
        <span>订阅消息</span>
      </div>
      <div class="item9">
        <img
          src="../assets/img/sale_icon9.png"
          width="45px"
          height="40px"
        >
        <span>短信</span>
      </div>
      <div class="item10">
        <img
          src="../assets/img/sale_icon10.png"
          width="45px"
          height="40px"
        >
        <span>智能触达</span>
      </div>
    </div>
  </div>
</template>
<style scoped>
.sale {
  width: 520px;
  height: 400px;
  position: absolute;
  display: flex;
}
.chang {
  width: 520px;
  height: 190px;
  position: absolute;
  display: flex;
  border: 1px solid rgba(189, 209, 255, 1);
  border-radius: 8px;
}
.chuda {
  width: 520px;
  height: 190px;
  top: 210px;
  position: absolute;
  display: flex;
  border: 1px solid rgba(189, 209, 255, 1);
  border-radius: 8px;
}
.title {
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
.btn_group {
  position: absolute;
  display: flex;
  width: 300px;
  height: 30px;
  top: 50px;
  left: 110px;
  justify-content: center;
  align-items: center;
  border: 2px solid rgba(199, 208, 255, 1);
  border-radius: 10px;
}
.button1,
.button2,
.button3 {
  font-size: 14px;
  display: flex;
  width: 100px;
  height: 30px;
  justify-content: center;
  align-items: center;
}
.button1 {
  background-color: rgba(112, 135, 250, 1);
  border-radius: 10px 0px 0px 10px;
}
.item1 {
  position: absolute;
  top: 100px;
  left: 35px;
}
.item1 span {
  display: block;
  text-align: center;
  color: gray;
}
.item2 {
  position: absolute;
  top: 100px;
  left: 125px;
}
.item2 span {
  display: block;
  text-align: center;
}
.item3 {
  position: absolute;
  top: 100px;
  left: 215px;
}
.item3 span {
  display: block;
  text-align: center;
  color: gray;
}
.item4 {
  position: absolute;
  top: 100px;
  left: 305px;
}
.item4 span {
  display: block;
  text-align: center;
  color: gray;
}
.item5 {
  position: absolute;
  top: 100px;
  left: 395px;
}
.item5 span {
  display: block;
  text-align: center;
  color: gray;
}
.item6 {
  position: absolute;
  top: 80px;
  left: 35px;
}
.item6 span {
  display: block;
  text-align: center;
}
.item7 {
  position: absolute;
  top: 80px;
  left: 125px;
}
.item7 span {
  display: block;
  text-align: center;
  color: gray;
}
.item8 {
  position: absolute;
  top: 80px;
  left: 215px;
}
.item8 span {
  display: block;
  text-align: center;
  color: gray;
}
.item9 {
  position: absolute;
  top: 80px;
  left: 305px;
}
.item9 span {
  display: block;
  text-align: center;
  color: gray;
}
.item10 {
  position: absolute;
  top: 80px;
  left: 395px;
}
.item10 span {
  display: block;
  text-align: center;
  color: gray;
}
</style>
