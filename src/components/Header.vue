<template>
  <header class="app-header">
    <div class="container">
      <img alt="" class="logo" src="@/assets/images/logos/logo.svg" />
      <div class="links-container">
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="link"
        >
          Products
        </router-link>
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="link"
        >
          Pricing
        </router-link>
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="link"
        >
          FAQ
        </router-link>
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="link"
        >
          Blog
        </router-link>
      </div>
      <div class="container-sing">
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="sign-in-link"
        >
          Sign in
        </router-link>
        <router-link
            :to="{name: 'MainPage'}"
            active="onclick"
            class="sign-up-link"
        >
          Sign up
        </router-link>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
}
</script>

<style scoped lang="scss">
.app-header {
  position: relative;
  z-index: 5;
  margin-left: auto;
  margin-right: auto;
  .container {
    background: transparent;
    height: 40px;
    z-index: 1;
    padding: 50px 210px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  .logo {
    height: 40px;
  }
  .links-container {
    height: 100%;
    display: flex;
    align-items: center;
    margin-left: 95px;
  }
  .link, .sign-up-link, .sign-in-link {
    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    color: #8794BA;
    margin-right: 36px;
    cursor: pointer;
  }

  .container-sing {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-right: 0;
    margin-left: auto;

    .sign-in-link {
      margin-right: 40px;
      width: 50px;
    }

    .sign-up-link {
      border: 1px solid #465B95;
      border-radius: 68px;
      width: 161px;
      padding: 10px 53px;
      margin-right: 0;
    }
  }
}
</style>
