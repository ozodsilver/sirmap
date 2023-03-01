<script setup>
 import Slider from '@vueform/slider'
import navbarVue from "./navbar.vue";
import footerVue from "./footer.vue";
import { ref } from "vue";
let value = ref(20)
let active = ref(false);

const isActive = ref(true);
const hasError = ref(false);
const toggleMenu = () => {
  active.value = !active.value;
};

let active2 = ref(false);

const isActive2 = ref(true);
const hasError2 = ref(false);
const toggleMenu1 = () => {
  active2.value = !active2.value;
};
</script>

<template>
  <div class="position-relative">
    <navbarVue></navbarVue>

    <iframe
      src="https://yandex.uz/maps/-/CCUG7VgdwA"
      frameborder="0"
      class="w-100"
      style="height: 79vh"
    ></iframe>

    <div class="left">
     
      <div class="ish2" @click="toggleMenu1()">
        <i
          class="fas fa-angle-double-right  text-white"
          style="margin-top: 250px"
        ></i>
      </div>
    </div>

    

    <div :class="{ silider2: active2 }">
      <Slider v-model="value" orientation = 'vertical'  v-if="active2" style="width: 20px;" />
    </div>

    <footerVue></footerVue>
  </div>
</template>

<style  >

@import url('@vueform/slider/themes/default.css');

.left {
  width: 3%;
  height: 60vh;
  position: absolute;
  z-index: 9999;
  top: 18%;
}
.ish1 {
  width: 80%;
  height: 30vh;
  background-color: rgba(0, 128, 0, 0.824);
  border-radius: 0px 15px 15px 0px;
  cursor: pointer;
}
.ish2 {
  width: 40%;
  height: 60vh;
  background-color: rgba(255, 0, 0, 0.687);
  border-radius: 0px 15px 15px 0px;
  cursor: pointer;
}
.silider {
  width: 100px;
  height: 40vh;
  position: absolute;
  top: 18%;
  left: 3%;
  border-radius: 20px;
  background: rgba(0, 128, 0, 0.598);
  backdrop-filter: blur(8px);
  overflow: hidden;
}
.form-range {
  transform: rotate(90deg);
  width: 300%;
  position: absolute;
  top: 45%;
  left: -100%;
}

.silider2 {
  width: 100px;
  height: 40vh;
  position: absolute;
  top: 23%;
  left: 2%;
  border-radius: 20px;
  background: rgba(255, 0, 0, 0.696);
  backdrop-filter: blur(8px);
  overflow: hidden;
  display: flex;
  justify-content: center; 
  align-items: center
}

@import url('vueform/slider/themes/default.css');
</style>
