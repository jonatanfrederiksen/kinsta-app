<script setup>
import Navmenu from './components/Navmenu.vue';

</script>


<style>
main {
  max-width: calc(100vw - 6rem);
  margin: 6em auto 5em;

}

.gradient {
  background: linear-gradient(45deg, #264653, #2a9d8f, #e9c46a, #f4a261, #e76f51);
  background-size: 600% 100%;
  animation: gradient 18s linear infinite;
  animation-direction: alternate;
  width: 100%;
  max-height: 600px;
  border-radius: 3em;
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

/* header {
  position: fixed;
  top: 1em;
  left: 0;
  right: 0;
  margin: 0 auto;
  z-index: 50;
} */

header>.wrap {
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

.site-title {
  font-family: "Honk", system-ui;
  line-height: 1.25;
}

header nav ul {
  display: flex;
  gap: 1em;
  list-style: none;
  padding: 0;
  margin: 0;
}

header span.btn a {
  padding: .7em 1.5em;
}

span.btn a {
  padding: 1em 1.5em;
  border-radius: 2em;
  background: #0003;
  
  text-decoration: none;
  transition: background .3s;
}

span.btn a:hover {
  background-color: #0005;
}


@media screen and (max-width: 479px) {

  /* header,
  .gradient {
    max-width: calc(100vw - 2rem);
  } */

  header .site-title {
    font-size: 1.5em;
  }

  span.btn a {
    padding: .5em 1em;
  }
}


</style>

<template>
  <div class=" ">

    <!-- <Navmenu title="Menu"></Navmenu> -->

    <header class="px-6 fixed top-4 z-10 w-full">
      <div class="wrap w-full max-w-2xl flex gap-4 justify-between">
        <a class="site-title text-3xl" href="/">Jon.atan.dk</a>

        <nav>
          <ul>
            <!-- <li class=" wp-block-navigation-item wp-block-navigation-link"><a class="wp-block-navigation-item__content"
                href="#hello"><span class="wp-block-navigation-item__label">Hej</span></a></li>
            <li class=" wp-block-navigation-item wp-block-navigation-link"><a class="wp-block-navigation-item__content"
                href="#projects"><span class="wp-block-navigation-item__label">Projekter</span></a></li> -->
          </ul>
        </nav>


        <span class="btn"><a href="mailto:jon@atan.dk">Kontakt</a></span>

      </div>
    </header>

    <main class="w-full max-w-screen-xl px-6">

      <div class="gradient flex items-center justify-center h-screen grow p-4 relative text-white w-full">
        <div class="flex flex-col md:flex-row items-center gap-4 w-full justify-evenly px-20">

          <img class="rounded-full w-40 md:w-1/4 min-w-20 max-w-sm drop-shadow-lg"
            src="./assets/jonatan-gradient-green.jpg" alt="">
          <div class="text-center ">
            <h1 class="mb-3 text-2xl md:text-4xl">Jonatan L. Frederiksen</h1>

            <ul class="flex gap-2 flex-wrap max-w-md justify-center">

              <li>
                <svg class=" inline w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
                  <path fill="currentcolor"
                    d="M483 159.7c10.9-24.6 21.4-60.4 21.4-87.9 0-72.7-79.6-98.4-209.7-38.6-107.6-7.2-211.2 73.7-237.1 186.5 30.9-34.9 78.3-82.3 122-101.2C125.4 166.9 79.1 228 44 291.7 23.2 329.7 0 390.9 0 436.7c0 98.6 92.9 86.5 180.3 42 31.4 15.4 66.6 15.6 101.7 15.6 97.1 0 184.2-54.3 216.8-146H377.9c-52.5 88.6-196.8 53-196.8-47.4H509.9c6.4-43.6-1.7-95.7-26.9-141.2zM64.6 346.9c17.7 51.2 53.7 95.9 100.3 123.3-88.7 48.9-173.3 29.1-100.3-123.3zm116-108.9c2-55.2 50.3-94.9 104-94.9 53.4 0 102 39.7 104 94.9H180.5zm184.5-187.6c21.4-10.3 48.6-22 72.6-22 31.4 0 54.3 21.7 54.3 53.7 0 20-7.4 49-14.6 67.9-26.3-42.3-66-81.6-112.3-99.6z" />
                </svg> web developer
              </li>

              <li>

                <svg class=" inline w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
                  <path fill="currentcolor"
                    d="M88 0C74.7 0 64 10.7 64 24c0 38.9 23.4 59.4 39.1 73.1l1.1 1C120.5 112.3 128 119.9 128 136c0 13.3 10.7 24 24 24s24-10.7 24-24c0-38.9-23.4-59.4-39.1-73.1l-1.1-1C119.5 47.7 112 40.1 112 24c0-13.3-10.7-24-24-24zM32 192c-17.7 0-32 14.3-32 32V416c0 53 43 96 96 96H288c53 0 96-43 96-96h16c61.9 0 112-50.1 112-112s-50.1-112-112-112H352 32zm352 64h16c26.5 0 48 21.5 48 48s-21.5 48-48 48H384V256zM224 24c0-13.3-10.7-24-24-24s-24 10.7-24 24c0 38.9 23.4 59.4 39.1 73.1l1.1 1C232.5 112.3 240 119.9 240 136c0 13.3 10.7 24 24 24s24-10.7 24-24c0-38.9-23.4-59.4-39.1-73.1l-1.1-1C231.5 47.7 224 40.1 224 24z" />
                </svg>
                coffee nerd
              </li>


            </ul>


            <div class="text-md mt-10 flex justify-center gap-2">

              <a class="p-4 bg-slate-800 opacity-75 hover:opacity-100 transition-opacity rounded-full flex justify-center items-center "
                href="mailto:jon@atan.dk"><img class="w-4" src="./assets/plane.svg" alt=""></a>
              <a class="p-4 bg-slate-800 opacity-75 hover:opacity-100 transition-opacity rounded-full flex justify-center items-center "
                href="https://www.linkedin.com/in/jonatan-lundager-frederiksen-695959103/" target="_blank"><img
                  class="w-4" src="./assets/linkedin-in.svg" alt=""></a>

            </div>

          </div>

        </div>

      </div>

      <section class="bg-white mt-20 ">
        <div class="mx-auto max-w-screen-xl px-4 md:px-12">
          <div class="grid gap-8 md:grid-cols-2 lg:gap-12">
            <div>
              <div class="gradient h-20 overflow-hidden rounded-xl bg-gray-100 shadow-lg md:h-auto border">
                <img
                  src="./assets/tetris-windows.jpg"
                  loading="lazy" alt="Photo by Martin Sanchez" class="h-full w-full object-cover object-center" />
              </div>
            </div>

            <div class="md:py-4 my-auto">
              <p class="text-center font-bold text-indigo-500 md:text-left">Welcome to my corner of the internet</p>

              <h1 class="mb-4 text-center text-2xl font-bold text-gray-800 sm:text-3xl md:mb-6 md:text-left">Play my <span style="font-family: 'Shadows Into Light', cursive;">TETRIS</span> game</h1>

              <p class="mb-6 text-gray-500 sm:text-lg md:mb-8 text-center md:text-start max-w-32 md:max-w-none">In 2021 i built my first Javascript game, since then i've learnt a lot, but it's still a lot of fun!</p>

              <p class="text-center md:text-start">
                <span class="btn text-white"><a href="https://jonatanfrederiksen.github.io/TETRIS/index.html" target="_blank">Try it out</a></span>
              </p>

            </div>
          </div>
        </div>
      </section>

    </main>

    <footer class="p-4 bg-white md:p-8 lg:p-10 dark:bg-gray-800">
  <div class="mx-auto max-w-screen-xl text-center">
      <a href="#" class="flex justify-center items-center text-2xl font-semibold text-gray-900 dark:text-white">
          
        <a class="site-title text-4xl" href="/">Jon.atan.dk</a>
    
      </a>
      <p class="my-6 text-gray-500 dark:text-gray-400">Creative fullstack web developer. <br>Email me at <a class="hover:underline" href="mailto:jon@atan.dk">jon@atan.dk</a>.</p>
      <!-- <ul class="flex flex-wrap justify-center items-center mb-6 text-gray-900 dark:text-white">
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6 ">About</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6">Premium</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6 ">Campaigns</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6">Blog</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6">Affiliate Program</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6">FAQs</a>
          </li>
          <li>
              <a href="#" class="mr-4 hover:underline md:mr-6">Contact</a>
          </li>
      </ul> -->
      <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">© {{ new Date().getFullYear() }}. All Rights Reserved.</span>
  </div>
</footer>


  </div>
</template>
