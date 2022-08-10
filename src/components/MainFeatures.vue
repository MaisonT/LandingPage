<template>
  <div class="main-features-block">
    <h1>Main Features</h1>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Elementum nisi aliquet volutpat pellentesque volutpat est.
      Sapien in etiam vitae nibh nunc mattis imperdiet sed nullam.
      Vitae et, tortor pulvinar risus pulvinar sit amet. Id vel in nam malesuada.
    </p>
    <div class="container">
      <div class="container-mini">
        <img alt="" src="@/assets/images/clock.svg" />
        <h2>Monitoring 24/7</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipis
          cing elit. Elementum nisi aliquet volutpat.
        </p>
      </div>

      <div class="container-mini">
        <img alt="" src="@/assets/images/monitor.svg" />
        <h2>Widget System</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipis
          cing elit. Elementum nisi aliquet volutpat.
        </p>
      </div>

      <div class="container-mini">
        <img alt="" src="@/assets/images/rocket.svg" />
        <h2>Best Performance</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipis
          cing elit. Elementum nisi aliquet volutpat.
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "MainFeatures"
}
</script>

<style scoped lang="scss">
.main-features-block {
  width: 1180px;
  margin-right: auto;
  margin-left: auto;
  padding: 55px 0 180px 0;

  h1 {
    font-style: normal;
    font-weight: 700;
    font-size: 40px;
    line-height: 47px;
    text-align: center;
    color: #E5E5E5;
    margin: 0 0 30px 0;
  }
  h2 {
    font-weight: 700;
    font-size: 16px;
    line-height: 19px;
    text-align: center;
    color: #E5E5E5;
  }
  p {
    font-weight: 400;
    font-size: 18px;
    text-align: center;
    color: #8794BA;
    margin-bottom: 81px;
  }
  .container {
    margin-right: auto;
    margin-left: auto;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 1180px;
    height: 164px;

    .container-mini {
      width: 380px;;
    }
  }
}
</style>