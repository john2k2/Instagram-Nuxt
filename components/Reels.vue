<script setup>
import data from "@/reels.json";

const translate = ref(0);

const next = () => {
  if (translate.value === 0) translate.value = 500;
  else if (translate.value === length * 500) translate.value = 0;
  else translate.value += 500;
};

const prev = () => {
  if (translate.value === 0) {
    translate.value = 0;
  } else {
    translate.value -= 500;
  }
};
</script>

<template>
  <div class="text-white flex gap-x-4 overflow-scroll relative z-10">
    <div
      class="mt-20 w-12 h-full flex-shrink-0 trabsition-transform duration-300 ease-in-out"
      v-for="reel in data"
      :key="reel.id"
      :style="{ transform: `translateX(-${translate}%)` }">
      <ul>
        <li class="w-full">
          <img :src="reel.imagen" alt="reel" class="object-cover rounded-full" />
          <h2 class="truncate text-nowrap text-xs">{{ reel.usuario }}</h2>
        </li>
      </ul>
    </div>
  </div>
  <div class="absolute top-0 left-0 z-50 w-full md:flex justify-between items-center mt-24 bg-transparent hidden px-2">
    <span
      @click="prev"
      class="pi pi-angle-left bg-white/90 rounded-full z-50 cursor-pointer"
      style="font-size: 1rem; color: black"></span>
    <span
      @click="next"
      class="pi z-50 pi-angle-right bg-white/90 rounded-full cursor-pointer"
      style="font-size: 1rem; color: black"></span>
  </div>
</template>

<style scoped></style>
