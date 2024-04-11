<script setup>
import Post from "@/photos-data";
</script>

<template>
  <section class="bg-white mt-6 w-full">
    <div v-for="(insta, index) in Post" :key="index">
      <div>
        <div class="flex items-center w-full px-3 mx-auto gap-x-4 mb-2">
          <img :src="insta.avatar" alt="avatar" class="object-cover rounded-full w-8 h-8" />
          <span class="text-sm text-white font-bold">{{ insta.nombre }}</span>
          <div class="justify-end flex w-full">
            <span class="pi pi-ellipsis-h" style="font-size: 1rem; color: white"></span>
          </div>
        </div>
        <div class="flex">
          <img :src="insta.imagen" alt="post" class="object-cover w-full" />
          <h2 class="text-sm text-red-500">{{ insta.usuario }}</h2>
        </div>
      </div>
      <div class="px-2 mx-auto py-4 grid grid-cols-10 gap-x-2">
        <div class="flex gap-x-4 col-span-8">
          <span class="pi pi-heart" style="font-size: 1.5rem; color: white"></span>
          <span class="pi pi-comment" style="font-size: 1.5rem; color: white"></span>
        </div>
        <div class="col-span-2 items-center grid justify-end">
          <span class="pi pi-bookmark" style="font-size: 1.5rem; color: white"></span>
        </div>
        <p class="text-white col-span-10 font-bold pt-2 capitalize text-sm">{{ insta.likes }} Me gusta</p>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
