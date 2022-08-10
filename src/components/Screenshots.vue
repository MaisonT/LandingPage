<template>
<div class="screenshots">
  <div class="container">
    <div class="container-mini">
      <div class="text-info">
        <h2>
          Automated Reports
          & Widget Alerts
        </h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          Elementum nisi aliquet volutpat pellentesque volutpat est.
          Sapien in etiam vitae nibh nunc mattis imperdiet sed nullam.
          Vitae et, tortor pulvinar risus pulvinar sit amet.
        </p>
      </div>
      <img alt="" src="@/assets/images/screenshots/screen01.svg"/>
    </div>

    <div class="container-mini">
      <img alt="" src="@/assets/images/screenshots/screen02.svg"/>
      <div class="text-info">
        <h2>
          Fully customizable to address your needs
        </h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          Elementum nisi aliquet volutpat pellentesque volutpat est.
          Sapien in etiam vitae nibh nunc mattis imperdiet sed nullam.
          Vitae et, tortor pulvinar risus pulvinar sit amet.
        </p>
      </div>
    </div>

    <div class="container-mini" style="margin-bottom: 0;">
      <div class="text-info">
        <h2>
          Pre-built Dashboard Templates
        </h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          Elementum nisi aliquet volutpat pellentesque volutpat est.
          Sapien in etiam vitae nibh nunc mattis imperdiet sed nullam.
          Vitae et, tortor pulvinar risus pulvinar sit amet.
        </p>
      </div>
      <img alt="" src="@/assets/images/screenshots/screen03.svg"/>
    </div>
  </div>
  <div id="pink"/>
  <div id="blue"/>
</div>
</template>

<script>
export default {
  name: "ScreenshotsInfo"
}
</script>

<style scoped lang="scss">
.screenshots {
  width: 100%;
  background: #E5E5E5;
}
.container {
  width: 1180.26px;
  height: 1800px;
  padding-top: 120px;
  padding-bottom: 120px;
  margin-left: auto;
  margin-right: auto;

  h2 {
    color: black;
    text-align: left;
    font-weight: 700;
    font-size: 40px;
    line-height: 47px;
  }
  p {
    text-align: left;
  }
  .container-mini {
    margin-bottom: 120px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    .text-info {
      width: 480px;
      margin-top: auto;
      margin-bottom: auto;
    }
  }
}
#pink {
  position: absolute;
  top: 3340px;
  left: 0;
  right: 0;
  height: 281px;
  width: 100%;
  max-width: none;
  background: #EF2A82;
  clip-path: polygon(100% 0, 0% 100%, 100% 100%);
  transform: rotate(0.1deg);
}
#blue {
  position: absolute;
  height: 281px;
  width: 100%;
  max-width: none;
  clip-path: polygon(100% 0, 0% 100%, 100% 100%);
  transform: rotate(0.8deg);
  background: #172755;
  top: 3351px;
}
</style>