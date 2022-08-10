<template>
  <AppHeader :scroll="scroll" :scrollTo="scrollTo" />
  <IntroductionInfo id="introduction"/>
  <hr id="pink"/>
   <div class="bg-logos">
    <img class="bg-logo-small" src="@/assets/images/logos/bg_logo_small.svg" alt="" />
    <img class="bg-logo-medium" src="@/assets/images/logos/bg_logo_medium.svg" alt="" />
    <img class="bg-logo-large" src="@/assets/images/logos/bg_logo_large.svg" alt="" />
  </div>
  <MainFeatures id="main-features" />
  <ScreenshotsInfo/>
  <PricingPlan id="prices"/>
  <AppFooter :scroll="scroll" :scrollTo="scrollTo" />
</template>

<script>
import AppHeader from './components/Header.vue'
import IntroductionInfo from "@/components/IntroductionInfo";
import MainFeatures from "@/components/MainFeatures";
import ScreenshotsInfo from "@/components/Screenshots";
import PricingPlan from "@/components/PricingPlan";
import AppFooter from "@/components/Footer";

export default {
  name: 'App',
  data() {
    return {
      scrollTo: {
        introduction: {
          name: 'Try for free',
          scroll: 'introduction',
        },
        features: {
          name: 'Main Features',
          scroll: 'features',
        },
        plans: {
          name: 'Pricing',
          scroll: 'prices',
        },
      }
    };
  },
  methods: {
    scroll(value) {
      if(value === 'introduction') {
        let el = document.getElementById("introduction");

        el.scrollIntoView({block: "center", behavior: "smooth"});
      }
      else if(value === 'prices') {
        let el = document.getElementById("prices");
        el.scrollIntoView({block: "center", behavior: "smooth"});
      }
      else if (value === 'features') {
        let el = document.getElementById("main-features");
        el.scrollIntoView({block: "center", behavior: "smooth"});
      }
    }
  },
  components: {
    AppFooter,
    PricingPlan,
    ScreenshotsInfo,
    MainFeatures,
    IntroductionInfo,
    AppHeader
  }
}
</script>

<style lang="scss">
html {
  background: #172755;
}
#app {
  font-family: Roboto, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100%;
  text-align: center;
  background: #172755;

  p {
    font-weight: 400;
    font-size: 18px;
    line-height: 150%;
    color: #8794BA;
  }

  .bg-logos {
    z-index: 1;
    .bg-logo-small {
      position: absolute;
      top: 0;
      left: 0;
    }

    .bg-logo-medium {
      position: absolute;
      right: 0;
      top: 0;
    }

    .bg-logo-large {
      position: absolute;
      right: 0;
      bottom: -20px;
    }
  }
  #pink {
    position: relative;
    border: none;
    height: 17px;
    background: #EF2A82;
  }
}
</style>