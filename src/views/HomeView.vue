<script setup lang="ts">
import collapse from '@/components/collapse.vue';
</script>

<template>
  <div class="resume">
    <div class="common-layout">
      <el-container>
        <!-- 顶部 -->
        <el-header class="header-with-background">


        </el-header>


        <el-container>
          <el-aside width="fit-content">
            <div class="title1">
              About me
            </div>
            <ul>
              <li class="item content">
                玩原神怎么你了
              </li>
            </ul>

            <div class="title1">
              Contact
            </div>
            <ul>
              <li class="item">
                Email <br>
                <span class="content">czdxwx@gmail.com</span><br>
                <span class="content">1226566881@qq.com</span>
              </li>

              <li class="item">
                Mobile <br><span class="content">18360830086</span>
              </li>

              <li class="item">
                Address <br>
                <span class="content">大丰区富强街<br>
                  江苏省盐城市<br>
                  中国</span>
              </li>
            </ul>

   

          </el-aside>


          <div class="split"></div>



          <el-main>
            <collapse/>
          </el-main>
        </el-container>
      </el-container>
    </div>


  </div>
</template>

<style scoped>
* {
  /* border: solid 1px black; */
  vertical-align: top;
  box-sizing: border-box;
  position: relative;
  font-family: 微軟正黑體;
}

.header-with-background {
  background-image: url('/src/assets/top.jpg');
  /* 替换成您的图片 URL */
  background-repeat: no-repeat;
  /* 防止背景图片重复 */
  background-position: center center;
  /* 将背景图片居中对齐 */
  /* 可以添加其他样式属性，如背景颜色、高度、边框等来定制您的头部样式 */
  height: 180px;
  /* 设置头部高度，根据您的需求进行调整 */
  overflow: hidden;

  z-index: 9999;
  /* 设置一个较高的 z-index 值 */
}

.resume {
  margin-top: 100px;
  border-radius: 8px;

  margin-left: auto;
  margin-right: auto;

  height: fit-content;
  width: 750px;
  background-color: #fffdf4;
  box-shadow: 5px 3px 20px rgba(0, 0, 0, 0.5);
  overflow: hidden;
}





.split {
  display: inline-block;
  width: 2px;
  height: 700px;
  top: -30px;
  border: solid 1px #c4a77f;
  border-style: dashed;
  border-left: none;
  border-top: none;
  border-bottom: none;

}

.left {
  display: inline-block;
  width: 40%;
  margin-right: 10px;
  height: 842px;
}

.title1 {
  display: inline-block;
  border: solid 5px #c68e43;

  height: 18px;
  width: 200px;
  margin-top: 25px;
  margin-left: 40px;
  border-top: none;
  border-right: none;
  border-bottom: none;
  padding-left: 10px;

  font-size: 0.9rem;
  font-weight: bold;
  color: #c68e43;
}

.item {
  list-style: none;
  font-size: 10px;
  font-weight: bold;
  margin-top: 20px;
  line-height: 15px;
  color: #333;
}

.content {
  font-size: 0.5rem;
  color: #333;
  top: 3px;
}

.chart {
  background-color: #ddd;
  height: 9px;
  width: 175px;
  margin-top: 2px;
  border-radius: 5px;
}

.Lheight2 {
  margin-top: 10px;
  line-height: 15px;
}

.value {
  background-color: #ddc4a1;
  height: 5px;
  top: 2px;
  left: 2px;
  border-radius: 5px;
}

.v1 {
  width: 85%;
}

.v2 {
  width: 75%;
}

.v3 {
  width: 80%;
}

.v4 {
  width: 80%;
}

.v5 {
  width: 65%;
}

.v6 {
  width: 95%;
}

.right {
  display: inline-block;
  width: 370px;
  height: 842px;
}

.Lheight3 {
  font-size: 8px;
  margin-top: 10px;
  line-height: 20px;
}

.Lheight4 {
  font-size: 6px;
  line-height: 10px;
  color: #8e8e8e;
}

.table {
  width: 400px;
}

.pie {
  top: 10px;
  display: inline-block;
  border-radius: 50%;
  margin-top: 0px;
  text-align: center;
  margin-right: 35px;
  width: 80px;
  height: 80px;

  overflow: hidden;
}

.pichart {
  width: 80px;
  height: 80px;
  background-color: #ddc4a1;
  border-radius: 50%;
}

.square {
  width: 40px;
  height: 40px;

}

.gray1 {
  background-color: #e8e8e8;
  top: -40px;
  left: 40px;

  transform-origin: 0px 0px;
}

.brown1 {
  background-color: #ddc4a1;
  top: -80px;
  left: 40px;

  transform-origin: 0px 0px;
  transform: rotate(18deg);
}

.brown2 {
  background-color: #ddc4a1;
  top: -80px;
  left: 40px;

  transform-origin: 0px 0px;
  transform: rotate(80deg);
}

.gray2 {
  background-color: #e8e8e8;
  top: -120px;
  left: 0px;
  height: 80px;

  transform-origin: 0px 0px;
}

.text {
  top: 22px;
}

.percent {
  top: 2px;
  font-size: 12px;
  color: #8e8e8e;
}


.circle {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  top: -155px;
  left: 5px;
  background-color: #fffdf4;
  line-height: 15px;
}

.c2 {
  top: -195px;
}

.move {
  top: 6px;
}

.page_title {
  height: 150px;
  text-align: center;
  top: 50px;
}

.title_content {
  top: 20px;
  font-size: 10px;
  left: 20px;
  margin-right: 40px;
}
</style>
