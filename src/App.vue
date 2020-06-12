<template>
  <div id="app">
    <HeaderNonAuthorized/>
    <HeaderAuthorized/>
    <!--img alt="Vue logo" src="./assets/logo.png"-->
    <!--HelloWorld msg="Welcome to Your Vue.js App"/-->
    <!--Temp/-->
    <Authorization/>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import Temp from "@/components/Temp";
import HeaderNonAuthorized from "@/components/HeaderNonAuthorized";
import Authorization from "@/components/Authorization";
import HeaderAuthorized from "@/components/HeaderAuthorized";

export default {
  name: 'App',
  components: {
    //HelloWorld,
    //Temp,
    HeaderNonAuthorized,
    Authorization,
    HeaderAuthorized

  }
}
</script>


<style>
#app {
 font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
 /* margin-top: 60px;*/


}
</style>
