<script setup>
import Navmenu from './components/Navmenu.vue';

</script>

<template>
  <div class="flex bg-slate-200 p-4">

    <!-- <Navmenu title="Menu"></Navmenu> -->


    <div class="flex items-center justify-center h-screen grow">
      <div class="flex flex-col text-center">
        <a class="mx-auto mb-6 inline text-center relative" href="mailto:frederiksen.jonatan@gmail.com">
          <img class="w-20 rounded-full hover:opacity-50 shadow-md transition-opacity" src="./assets/profile.jpeg" alt="">
          <span
            class="opacity-0 absolute inset-0 flex justify-center align-center transition-opacity hover:opacity-100"><img
              class="w-7" src="./assets/plane.svg" alt=""></span>
        </a>
        <h1 class="mb-3 text-4xl">Jonatan Lundager Frederiksen</h1>
        <p class="text-lg max-w-full ">Fullstack webdeveloper</p>

      </div>
    </div>
  </div>
</template>
