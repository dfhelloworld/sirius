<template>
  <div class="wrapper">
    <image
      :src="logo"
      class="logo"
    />
    <text class="greeting">The environment is ready!</text>
    <router-view />
    <footer></footer>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      logo: "https://gw.alicdn.com/tfs/TB1yopEdgoQMeJjy1XaXXcSsFXa-640-302.png"
    };
  }
};
</script>

<style lang="scss">
@import "./style/common";
.router-fade-enter-active,
.router-fade-leave-active {
  transition: opacity 0.3s;
}
.router-fade-enter,
.router-fade-leave-active {
  opacity: 0;
}
</style>
