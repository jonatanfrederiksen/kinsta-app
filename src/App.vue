<script setup>
import Navmenu from './components/Navmenu.vue';

</script>
<style>
.gradient {
  width: 100%;
  height: 100%;
  position: absolute;
  background: linear-gradient(45deg, #264653, #2a9d8f, #e9c46a, #f4a261, #e76f51);
  background-size: 600% 100%;
  animation: gradient 18s linear infinite;
  animation-direction: alternate;
}

@keyframes gradient {
  0% {
    background-position: 0%
  }

  100% {
    background-position: 100%
  }
}
</style>
<template>
  <div class="flex bg-slate-200 ">

    <!-- <Navmenu title="Menu"></Navmenu> -->


    <div class="gradient flex items-center justify-center h-screen grow p-4 relative text-white">
      <div class=""></div>
      <div class="flex flex-col text-center">
        <a class="mx-auto mb-6 inline text-center relative" href="mailto:frederiksen.jonatan@gmail.com">
          <img class="w-20 rounded-full hover:opacity-50 shadow-md transition-opacity" src="./assets/profile.jpeg" alt="">
          <span
            class="opacity-0 absolute inset-0 flex justify-center align-center transition-opacity hover:opacity-100"><img
              class="w-5" src="./assets/plane.svg" alt=""></span>
        </a>
        <h1 class="mb-3 text-4xl">Jonatan Lundager Frederiksen</h1>
        <p class="text-lg max-w-full ">Fullstack webdeveloper</p>

      </div>
    </div>
</div></template>
