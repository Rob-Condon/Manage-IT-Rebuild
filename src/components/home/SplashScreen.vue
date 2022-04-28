<template>
  <div class="flex-auto flex ph7 ph0-m">
    <div style="width: 100%; height: 70vh; text-align: left; display: flex; flex-direction: column; justify-content: center">
      <h1 class="display-1 title pa2">The DevOps Platform has arrived.</h1>
      <h3 class="display-3 subTitle pa2">Deliver software faster with better security and collaboration in a single platform..</h3>
      <div>
        <va-button class="va-button--active ma=3"> Go </va-button>
        <va-button class="va-button--default ma-3" color="warning"> Services</va-button>
      </div>
    </div>
    <div style="width: 100%; height: 500px;"></div>
  </div>
</template>

<script>
import {VaButton} from "vuestic-ui";
export default {
  name: "SplashScreen",
  components: {VaButton}
}
</script>

<style scoped>
.title {
  font-family: 'Raleway', sans-serif;
  font-weight: 300;
}
.subTitle {
  font-family: 'Raleway', sans-serif;
  font-weight: 200;
}
</style>