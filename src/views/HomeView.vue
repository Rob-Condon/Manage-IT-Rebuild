<template>
  <SplashScreen/>
  <BaseInfo/>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import SplashScreen from "@/components/home/SplashScreen";
import BaseInfo from "@/components/home/infomation/BaseInfo";

export default {
  name: 'HomeView',
  components: {
    BaseInfo,
    SplashScreen,
    HelloWorld
  }
}
</script>
