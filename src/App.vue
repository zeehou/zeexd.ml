<template>
  <div id="app">
    <n-back-top :right="100" />
    <header>
      <h1 class="animate__animated animate__jello">Counter-Strike: Global Offensive</h1>
      <!-- <h1>Config</h1> -->
     

      <div class="test" >
        <n-card
          id="config"
          class="animate__animated animate__jello"
          title="Config" 
          hoverable
          :segmented="{
            content: 'hard',
            footer: 'soft',
          }"
        >
          <div class="c1">
            <n-tooltip trigger="hover" placement="top-start">
              <template #trigger> <span class="animate__animated animate__flip">游戏：</span></template>
              请尽量把右方的两个cfg文件都放置在<br>csgo根目录下的cfg文件夹内 </n-tooltip
            ><n-button class="btnconfig animate__animated animate__jello btnani" tag="a" href="cfg/wb.cfg"
              >Config</n-button
            >

            <n-button class="btnani" tag="a" href="cfg/autoexec.cfg">AutoExec</n-button>
          </div>
          <div>
            练习：<n-button class="btnconfig btnani" tag="a" href="cfg/bot1.cfg"
              >Bot1</n-button
            >
            <n-button class="btnconfig btnani" tag="a" href="cfg/bot2.cfg"
              >Bot2</n-button
            >
            <n-button class="btnani" tag="a" href="cfg/train.cfg">Train</n-button>
          </div>

          <div></div>
        </n-card>
        <n-card
          id="config"
          class="animate__animated animate__jello"
          title="Test"
          hoverable
          :segmented="{
            content: 'hard',
            footer: 'soft',
          }"
        >
          <div class="c1">
            媒体测试：<n-button class="btnani" tag="a" href="https://www.onlinemictest.com/zh/"
              >Mic Test</n-button
            >
          </div>

          <div>
            鼠标测试：<n-button
              class="btnconfig btnani"
              tag="a"
              href="tool/MouseRateChecker.rar"
              >RateTest</n-button
            >
            <n-button class="btnani" tag="a" href="tool/MouseTest.zip">MouseTest</n-button>
          </div>
        </n-card>
      </div>
    </header>

    <h2 class="animate__animated animate__backInUp">Pro Config：</h2>

    <crosshair class="animate__animated animate__backInUp" />



     
  </div>



 
</template>


<script>

// import HelloWorld from './components/HelloWorld.vue';
import crosshair from "./components/crosshair.vue";
import { NButton, NBackTop, NCard, NTooltip } from "naive-ui";
// import anime from 'animejs';


export default {
  name: "App",
  components: {
    // HelloWorld,

    crosshair,
    NButton,
    NBackTop,
    NCard,
    NTooltip,
  
  },
};

</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Oswald:300,400,700);
@import url(https://fonts.googleapis.com/css?family=Source+Sans+Pro:200,300,400,600,700,900,200italic,300italic,400italic,600italic,700italic,900italic);

#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  font-family: "Oswald", sans-serif;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  margin: 20px;
}
body {
  background-color: rgba(136, 136, 136, 0.041);
}

.c1 {
  margin-bottom: 5px;
}
.btnconfig {
  margin-right: 5px;
}

#config {
  width: 400px;
  margin: 5px;
  /* margin: 0 auto; */
}
.test {
  display: flex;
  /* flex-direction: column; */
  flex-wrap: wrap;
  justify-content: center;
}
.btnani{
  animation: jello;
  animation-duration: 1s;
  width: 60px!important
}
.btnani:focus{
  animation: bounceIn ;
  animation-duration: 2s;

}



/* .animate__animated.animate__bounce {
  --animate-duration: 2s;
} */
</style>
