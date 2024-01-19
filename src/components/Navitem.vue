<template>
    <a :href="link" class="flex flex-row justify-center items-center gap-3">
        <span class="w-32">{{ title }}</span>
        <img class="w-10 p-2 rounded-full hover:bg-slate-200" :src="'src/assets/' + icon" alt="Home" /></a>
</template>


<script>
export default {
    props: {
        title: String,
        link: String,
        icon: String,
    },
}
</script>