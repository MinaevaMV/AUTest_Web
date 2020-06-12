<template>
    <div id="app">
        <HeaderNonAuthorized/>
        <HeaderAuthorized/>
        <!--img alt="Vue logo" src="./assets/logo.png"-->
        <!--HelloWorld msg="Welcome to Your Vue.js App"/-->
        <!--Temp/-->
        <Authorization/>
        <AboutProject style="display:none" projectName="Autest"/>
        <TestSet style="display: none" set-name="Test-set 1. Авторизация"></TestSet>
    </div>
</template>

<script>
    //import HelloWorld from './components/HelloWorld.vue'
    //import Temp from "@/components/Temp";
    import HeaderNonAuthorized from "./components/HeaderNonAuthorized";
    import Authorization from "./components/Authorization";
    import HeaderAuthorized from "./components/HeaderAuthorized";
    import AboutProject from "./components/AboutProject";
    import TestSet from "./components/TestSet";

    export default {
        name: 'App',
        components: {
            TestSet,
            //HelloWorld,
            //Temp,
            HeaderNonAuthorized,
            Authorization,
            HeaderAuthorized,
            AboutProject

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
