<template>
  <div id="app">
    <header>
      <h1>Counter-Strike: Global Offensive!</h1>
      <!-- <h1>Config</h1> -->
      
      <div class="test">
        <n-card
          id="config"
          title="Config"
          hoverable
          :segmented="{
            content: 'hard',
            footer: 'soft',
          }"
        >
          <div class="c1">
            整合版(网吧)：<n-button tag="a" href="cfg/wb.cfg">wb.cfg</n-button>
          </div>

          <div>
            独立版(家里)：<n-button
              class="btnconfig"
              tag="a"
              href="cfg/config.cfg"
              >config</n-button
            >
            <n-button tag="a" href="cfg/autoexec.cfg">autoexec</n-button>
          </div>
        </n-card>
        <n-card
          id="config"
          title="Test"
          hoverable
          :segmented="{
            content: 'hard',
            footer: 'soft',
          }"
        >
          <div class="c1">
            媒体测试：<n-button tag="a" href="https://www.onlinemictest.com/zh/"
              >Mic Test</n-button
            >
          </div>

          <div>
            鼠标测试：<n-button
              class="btnconfig"
              tag="a"
              href="tool/MouseRateChecker.rar"
              >RateTest</n-button
            >
            <n-button tag="a" href="tool/MouseTest.zip">MouseTest</n-button>
          </div>
        </n-card>
      </div>
    </header>

    <h2>Pro Config：</h2>

    <crosshair />

    <n-back-top :right="40" />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import crosshair from "./components/crosshair.vue";
import { NButton, NBackTop, NCard } from "naive-ui";

export default {
  name: "App",
  components: {
    // HelloWorld,

    crosshair,
    NButton,
    NBackTop,
    NCard,
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
.n-button {
  width: 60px;
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
</style>
