<template>
  <div class="screen-bg">
    <!-- 头部标题部分 -->
    <div class="header">
      <div class="title">青海省生态环境保护修复项目平台</div>
      <div class="weather">
        <div class="weather-text">雷阵雨</div>
      </div>
      <div class="header-bottom"></div>
    </div>

    <!-- 内容部分 -->
    <div class="content">
      <!-- 左侧 -->
      <div class="left"></div>

      <!-- 中部 -->
      <div class="center">
        <div class="center-top"></div>
        <div class="center-bottom"></div>
      </div>

      <!-- 右侧 -->
      <div class="right">
        <div class="right-top"></div>
        <div class="right-bottom"></div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
  .screen-bg {
    display: flex;
    flex-direction: column;
    height: 100%;
    width: 100%;

    /* 背景 */
    background: url(@/assets/images/bg.png);
  }

  .header {
    display: flex;
    flex-direction: column;
    height: 103px;

    /* 头部背景 */
    background-image: url(@/assets/images/bg_header.png);

    .title {
      display: flex;
      padding-top: 14px;
      padding-left: 705px;
      font-size: 36px;
      font-family: PangMenZhengDao;
      color: #5BBBFE;
      line-height: 41px;
      letter-spacing: 1px;
      text-shadow: 0px 2px 0px #2E5E80;
      background: linear-gradient(180deg, #FFFFFF 0%, #5BBBFE 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .weather .weather-text {
      padding-left: 68px;
      padding-top: 16px;
      width: 42px;
      height: 20px;
      font-size: 14px;
      font-family: DINAlternate-Bold, DINAlternate;
      font-weight: bold;
      color: #E6F7FF;
      line-height: 16px;
    }

    .header-bottom {
      margin: 69px auto 0;
      width: 216px;
      height: 33px;
      background: linear-gradient(360deg, #2687D3 0%, rgba(85,239,255,0) 100%);
      border: 1px solid;
      border-image: linear-gradient(180deg, rgba(0, 175, 255, 0), rgba(0, 175, 255, 1)) 1 1;
      /* border-radius: 10px 10px;  */
    }
  }

  // 内容部分
  .content {
    display: flex;

    .left {
      display: flex;
      width: 428px;
      height: 961px;
      margin-left: 12px;

      background-image: url(@/assets/images/bg_left.png);
    }

    .center-top {
      width: 855px;
      height: 611px;
      background-image: url(@/assets/images/位图.png);

      margin-left: 81px;
      margin-top: 117px;
    }

    .center-bottom {
      // display: flex;
      width: 995px;
      height: 194px;

      background-image: url(@/assets/images/项目预警信息.png);

      margin-left: 21px;
      // margin-top: 5px; // 无效果
    }

    .right {
      display: flex;
      flex-direction: column;
      // width: 430px;
      // height: 977px;

      .right-top {
        width: 430px;
        height: 450px;

        background-image: url(@/assets/images/资金进度.png);
      }

      .right-bottom {
        width: 428px;
        height: 435px;

        background-image: url(@/assets/images/工程进度.png);

        margin-top: 62px;
        margin-left: 24px;
      }
    }
  }

</style>