<template>
  <div class="ai">
    <div class="title">
      <span style="font-size: 12px;">按店推荐</span>
    </div>
    <img
      src="../assets/img/ai.png"
      width="30px"
      height="30px"
    >
    <span style=" font-size: 20px; font-weight: 700;">AI匹配</span>
    <span style="font-size: 12px; font-weight: 700; position: absolute; top: 5px; left: 100px;">
      -智能生成匹配方案
    </span>
    <div class="item1">
      <img
        src="../assets/img/icon5.png"
        width="15px"
        height="15px"
      >
      <span style="color:rgba(10, 31, 55, 0.6); font-size: 12px; margin-left: 5px;">
        已使用ICF算法为23家门店生成人货匹配方案
      </span>
    </div>
    <div class="item2">
      <img
        src="../assets/img/icon5.png"
        width="15px"
        height="15px"
      >
      <span style="color:rgba(10, 31, 55, 0.6); font-size: 12px; margin-left: 5px;">
        推荐38款商品（1,344件库存）&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;推荐6,921人
      </span>
    </div>
    <button class="button1">更换算法⬇</button>
    <div class="item3">
      <span style="font-size:11px;color: gray;">畅销</span>
      <div style="width: 100px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">12款</span>
    </div>
    <div class="item4">
      <span style="font-size:11px;color: gray;">滞销</span>
      <div style="width: 80px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">5款</span>
    </div>
    <div class="item5">
      <span style="font-size:11px;color: gray;">平销</span>
      <div style="width: 110px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">15款</span>
    </div>
    <div class="item6">
      <span style="font-size:11px;color: gray;">重要价值</span>
      <div style="width: 100px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">2000人</span>
    </div>
    <div class="item7">
      <span style="font-size:11px;color: gray;">重要挽留</span>
      <div style="width: 40px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">1300人</span>
    </div>
    <div class="item8">
      <span style="font-size:11px;color: gray;">一般价值</span>
      <div style="width: 80px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">1800人</span>
    </div>
    <div class="item9">
      <span style="font-size:11px;color: gray;">一般挽留</span>
      <div style="width: 20px;height: 10px;background-color: rgba(138, 169, 252, 1);border-radius: 5px;"></div>
      <span style="font-size:11px;">821人</span>
    </div>
    <button class="button2">查看方案明细 ></button>
  </div>
</template>
<style scoped>
.ai {
  width: 520px;
  height: 250px;
  position: absolute;
  display: flex;
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
  top: -20px;
  right: -29px;
  opacity: 1;
  border-radius: 0px 8px 0px 16px;
  background: rgba(112, 135, 250, 1);
}
.item1 {
  position: absolute;
  top: 50px;
  left: 50px;
}
.item2 {
  position: absolute;
  top: 80px;
  left: 50px;
}
.item3 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 120px;
  left: 70px;
  align-items: center;
}
.item4 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 140px;
  left: 70px;
  align-items: center;
}
.item5 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 160px;
  left: 70px;
  align-items: center;
}
.item6 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 120px;
  left: 290px;
  align-items: center;
}
.item7 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 135px;
  left: 290px;
  align-items: center;
}
.item8 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 150px;
  left: 290px;
  align-items: center;
}
.item9 {
  display: flex;
  position: absolute;
  width: 200px;
  height: 20px;
  top: 165px;
  left: 290px;
  align-items: center;
}
.button1 {
  position: absolute;
  left: 330px;
  top: 52px;
  width: 70px;
  font-size: 11px;
  background-color: rgba(255, 248, 242, 1);
  border: 1px solid rgba(252, 151, 73, 1);
  border-radius: 10px;
  color: rgba(252, 151, 73, 1);
  cursor: pointer;
}
.button2 {
  position: absolute;
  cursor: pointer;
  bottom: 0;
  left: 200px;
  width: 100px;
  height: 30px;
  font-size: 12px;
  color: white;
  border: 0;
  border-radius: 10px;
  background-color: rgba(252, 151, 73, 1);
}
</style>