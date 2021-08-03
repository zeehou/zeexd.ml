<template>
  <div class="cross">
    <n-card
      class="crossbox2"
      title="S1mple"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshairgap -3; cl_crosshairsize 1; cl_crosshairalpha 250;
      cl_crosshaircolor 4; cl_crosshairdot 1; cl_crosshairstyle 4;
      cl_crosshairusealpha 1; cl_crosshairthickness 0; cl_crosshair_sniper_width
      1; cl_crosshair_drawoutline 0; cl_crosshaircolor_r 255;
      cl_crosshaircolor_g 255; cl_crosshaircolor_b 255;
      <template #footer
        ><n-button href='cfg/s1mple.zip' ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>

    <n-card
      class="crossbox2"
      title="B1t"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshair_drawoutline 0; cl_crosshair_sniper_width 1; cl_crosshairalpha
      255; cl_crosshaircolor 4; cl_crosshaircolor_b 144; cl_crosshaircolor_g
      238; cl_crosshaircolor_r 0; cl_crosshairdot 0; cl_crosshairgap -3;
      cl_crosshairsize 2; cl_crosshairstyle 4; cl_crosshairthickness 0;
      cl_crosshairusealpha 1;

      <template #footer
        ><n-button ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>

    <n-card
      class="crossbox2"
      title="NiKo"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshairalpha 255; cl_crosshaircolor 5; cl_crosshairdot 0;
      cl_crosshairgap -4; cl_crosshairsize 2; cl_crosshairstyle 4;
      cl_crosshairusealpha 1; cl_crosshairthickness 1; cl_crosshair_drawoutline
      0; cl_crosshair_sniper_width 1; cl_crosshaircolor_r 255;
      cl_crosshaircolor_g 255; cl_crosshaircolor_b 250;
      <template #footer
        ><n-button ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>

    <n-card
      class="crossbox2"
      title="arT"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshairalpha 255; cl_crosshaircolor 1; cl_crosshairdot 0;
      cl_crosshairgap -3; cl_crosshairsize 2; cl_crosshairstyle 4;
      cl_crosshairusealpha 1; cl_crosshairthickness 0; cl_crosshair_drawoutline
      0;

      <template #footer
        ><n-button ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>

    <n-card
      class="crossbox2"
      title="ZywOo"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshairsize 2; cl_crosshairstyle 4; cl_crosshairgap -3;
      cl_crosshairdot 0; cl_crosshairthickness 0; cl_crosshair_drawoutline 0;
      cl_crosshair_outlinethickness 0.5; cl_crosshaircolor 1;
      cl_crosshaircolor_r 255; cl_crosshaircolor_g 255; cl_crosshaircolor_b 255;
      cl_crosshair_sniper_width 1;

      <template #footer
        ><n-button ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>

    <n-card
      class="crossbox2"
      title="ropz"
      :segmented="{
        content: 'hard',
        footer: 'soft',
      }"
    >
      <template #header-extra></template>
      cl_crosshairalpha 250; cl_crosshaircolor 1; cl_crosshairdot 0;
      cl_crosshairgap -3; cl_crosshairsize 2; cl_crosshairstyle 4;
      cl_crosshairusealpha 1; cl_crosshairthickness 0; cl_crosshair_drawoutline
      0;
      <template #footer
        ><n-button ghost color="#ff69b4">Config</n-button></template
      >
    </n-card>
  </div>
</template>

<script>
import { NButton, NCard } from "naive-ui";

export default {
  name: "crosshair",
  components: {
    NButton,
    NCard,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* n-scrollbar{
  overflow: scroll;
  height: 100%;
} */
.crossbox {
  width: 260px;
}
.crossbox2 {
  width: 200px;
  margin: 5px;
  line-height: 130%;
  /* height: 300px; */
}

.light-green {
  height: 108px;
  background-color: rgba(0, 128, 0, 0.12);
  /* width: 200px; */
}
.green {
  height: 108px;
  background-color: rgba(0, 128, 0, 0.24);
  /* width: 200px; */
}
/* n-gi div{
  width: 200px;
} */
/* .gridbox{
  display: grid;
  grid-template-columns: repeat(2, 500px 20px 80px);
} */
.cross {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

</style>
