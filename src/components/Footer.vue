<template>
<div class="app-footer">
  <hr>
  <div class="footer-container">
    <img class="logo-transparent" src="@/assets/images/logos/logo_transparent.svg" alt="" />
    <div class="links-container">
      <div
          @click="scroll"
          active="onclick"
          class="link"
      >
        Products
      </div>
      <div
          @click="scroll"
          active="onclick"
          class="link"
      >
        Pricing
      </div>
      <div
          @click="scroll"
          active="onclick"
          class="link"
      >
        FAQ
      </div>
      <div
          @click="scroll"
          active="onclick"
          class="link"
      >
        Blog
      </div>
    </div>
    <div class="links-container">
      <a class="link" target="_blank" href="https://www.facebook.com/">
        <img src="@/assets/images/socialNetworks/facebook.svg" alt="" />
      </a>
      <a class="link" target="_blank" href="https://www.twitter.com/">
        <img src="@/assets/images/socialNetworks/twitter.svg" alt="" />
      </a>
      <a class="link" target="_blank" href="https://www.instagram.com/">
        <img src="@/assets/images/socialNetworks/instagram.svg" alt="" />
      </a>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "AppFooter",
  props: {
    linkName: String,
    linkRoute: String,
  },
  methods: {
    scroll() {
      window.scrollTo(0,0);
    }
  }
}
</script>

<style scoped lang="scss">
.app-footer {
  height: 196px;
  width: 1180px;
  margin-left: auto;
  margin-right: auto;

  hr {
    width: 1180px;
    height: 1px;
    background: #2A407C;
    border: none;
    margin-bottom: 63px;
  }

  .footer-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    .links-container {
      height: 100%;
      display: flex;
      align-items: center;

      div:active {
        background: rgba(28, 28, 28, 0.16);
      }
    }
    .link {
      font-weight: 400;
      font-size: 16px;
      line-height: 19px;
      color: #8794BA;
      margin-left: 40px;
      cursor: pointer;
    }

  }
}
</style>