<script setup lang="ts">
import logoDark from "~/assets/logo-dark.webp";
import logoWhite from "~/assets/logo-white.webp";

const title = "We'll be right back.";
const desc =
  "We seem to be facing some issues right now, but we're working overtime to solve and bring you the best experience possible!";

useHead({
  title: `SAFT Blog | ${title}`,
  meta: { name: "description", content: desc },
});
</script>

<template>
  <div
    class="grid bg-slate-50 dark:bg-slate-800 w-screen h-screen place-items-center px-5"
  >
    <div
      class="max-w-xl bg-slate-200 dark:bg-slate-900 rounded-lg h-fit p-10 text-center"
    >
      <img :src="logoDark" class="block dark:hidden w-52 mx-auto mb-7" />
      <img :src="logoWhite" class="hidden dark:block w-52 mx-auto mb-7" />
      <h1 class="text-3xl font-bold mb-3 text-slate-900 dark:text-slate-50">
        {{ title }}
      </h1>
      <p class="text-slate-900 text-lg dark:text-slate-50">
        {{ desc }}
      </p>
    </div>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;700&display=swap");

html {
  font-family: "Manrope", sans-serif;
}
</style>
