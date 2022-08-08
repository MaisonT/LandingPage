<template>
<div class="introduction-info">
  <div class="introduction-block">
    <h1>
      Monitor your business on real-time dashboard
    </h1>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Elementum nisi aliquet volutpat pellentesque volutpat est.
      Sapien in etiam vitae nibh nunc mattis imperdiet sed nullam.
    </p>
    <button>Try for free</button>
  </div>
  <img class="bg-logo-small" src="@/assets/images/screenshots/main_screen.svg" alt="" />
</div>
</template>

<script>
export default {
  name: "IntroductionInfo"
}
</script>

<style scoped lang="scss">
.introduction-info {
  background: #172755;
  padding-top: 102px;
  width: 1180px;
  height: 798px;
  z-index: 3;

  .bg-logo-small {
    z-index: 1;
    position: absolute;
    top: 164px;
    right: 0;
  }
}
.introduction-block {
  width: 560px;
  align-items: flex-start;
  margin-left: 210px;
  position: relative;
  z-index: 3;

  h1 {
    color: #FFFFFF;
    text-align: left;
    font-weight: 700;
    font-size: 50px;
    line-height: 120%;
  }
  p {
    text-align: left;
  }
  button {
    margin-top: 50px;
    margin-right: 100%;
    padding: 10px 80px;
    gap: 10px;

    width: 238px;
    height: 50px;

    background: #EF2A82;
    border-radius: 68px;
    border: none;

    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    color: #FFFFFF;
    cursor: pointer;

    &:hover {
      background: #EF1F99;
    }
  }
}
</style>