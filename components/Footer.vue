<script setup>
import Submit from "~/assets/icons/Submit.vue";
import Media from "~/assets/icons/Media.vue";
import Chat from "~/assets/icons/Chat.vue";
import Home from "~/assets/icons/Home.vue";
</script>

<template>
  <footer>
    <div class="fixed w-full z-50 bottom-0 py-3 border-t-[0.1px] border-white/30">
      <div class="flex justify-between items-center w-[80%] mx-auto">
        <Home class="w-[1.5rem] col-span-2" />
        <span class="pi pi-compass col-span-2" style="font-size: 1.5rem; color: white"></span>
        <Media class="w-[1.5rem] col-span-2" />
        <Submit class="w-[1.5rem] col-span-2" />
        <Chat class="w-[1.5rem] col-span-2" />
        <div class="w-[1.5rem] col-span-2">
          <img class="rounded-full w-full" src="/public/img/asset 2.jpeg" alt="" />
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped></style>
