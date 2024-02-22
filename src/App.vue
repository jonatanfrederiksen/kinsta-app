<script setup>
import Navmenu from './components/Navmenu.vue';

</script>
<style>
.gradient {
    background: linear-gradient(45deg, #264653, #2a9d8f, #e9c46a, #f4a261, #e76f51);
    background-size: 600% 100%;
    animation: gradient 18s linear infinite;
    animation-direction: alternate;
    width: 100%;
    max-width: calc(100vw - 6rem);
    max-height: 600px;
    border-radius: 3em;
    margin: 6em  auto 5em;
    box-shadow: 1px 1px 1px 2px #000;
}
@keyframes gradient {
  0% {
    background-position: 0%
  }

  100% {
    background-position: 100%
  }
}

header {
  position: fixed;
  top: 1em;
  left: 0;
  right: 0;
  max-width: min(700px, 100vw - 8rem);
  margin: 0 auto;
  z-index: 50;
}

header>.wrap {
  max-width: 700px;
  margin-inline: auto;
  position: sticky;
  top: 0;
  border-radius: 3em;
  backdrop-filter: blur(2em);
  background: #0003 !important;
  color: #fff;
  padding: .5em .5em .5em 2em !important;
  box-shadow: 0 0 11px -5px #0005;
  align-items: center;
}

header .site-title {
  font-family: "Honk", system-ui;
  font-size: 2.5em;
  line-height: 1.25;
}

header nav ul {
  display: flex;
  gap: 1em;
  list-style: none;
  padding: 0;
  margin: 0;
}

span.btn a {
  padding: 1em 1.5em;
  border-radius: 2em;
  background: #0003;
  color: #fff;
  text-decoration: none;
  transition: background .3s;
}
span.btn a:hover {
  background-color: #0005;
}


@media screen and (max-width: 479px){
  header,
  .gradient{
    max-width: calc(100vw - 2rem);
  }
  header .site-title{
    font-size: 1.5em;
  }

  span.btn a{
    padding: .5em 1em;
  }
}

</style>
<template>
  <div class="flex ">

    <!-- <Navmenu title="Menu"></Navmenu> -->

    <header>
      <div class="wrap flex gap-4 justify-between">
        <a class="site-title" href="/">Jonatan</a>

        <nav>
          <ul>
            <!-- <li class=" wp-block-navigation-item wp-block-navigation-link"><a class="wp-block-navigation-item__content"
                href="#hello"><span class="wp-block-navigation-item__label">Hej</span></a></li>
            <li class=" wp-block-navigation-item wp-block-navigation-link"><a class="wp-block-navigation-item__content"
                href="#projects"><span class="wp-block-navigation-item__label">Projekter</span></a></li> -->
          </ul>
        </nav>


        <span class="btn"><a href="mailto:frederiksen.jonatan@gmail.com?subject=Lad os arbejde sammen!&body=Hej Jonatan! %0D%0A%0D%0AJeg vil høre mere om ...">Kontakt</a></span>

      </div>
    </header>

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
  </div>
</template>
