<template>
    <div class="bg-gray-100 flex flex-col justify-start items-center p-4 pr-0">
        <h1 class="text-3xl font-bold pr-4 ">{{ title }}</h1>
        <Navitem title="Home" link="/" icon="home.svg"></Navitem>
        <Navitem title="Tetris" link="/tetris" icon="home.svg"></Navitem>
    </div>
</template>


<script>

import Navitem from './Navitem.vue';

export default {
    props: {
        title: String,
    },

    components: {
        Navitem,
    },
}
</script>