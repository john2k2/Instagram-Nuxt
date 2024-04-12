<script setup>
import Post from "@/photos-data";
import Comment from "~/assets/icons/Comment.vue";
import NotificationsChange from "~/assets/icons/NotificationsChange.vue";
import Save from "~/assets/icons/Save.vue";
</script>

<template>
  <section class="bg-white mt-6 w-full">
    <div v-for="insta in Post" :key="insta.id">
      <div>
        <div class="flex items-center w-full px-3 mx-auto gap-x-4 mb-2">
          <img :src="insta.avatar" alt="avatar" class="object-cover rounded-full w-8 z-10" />
          <span class="text-sm text-white font-bold">{{ insta.nombre }}</span>
          <div class="justify-end flex w-full">
            <span class="pi pi-ellipsis-h" style="font-size: 1rem; color: white"></span>
          </div>
        </div>
        <div class="flex w-full justify-center items-center">
          <div v-for="(img, index) in insta.imagen" :key="index" class="">
            <img :src="img.url" alt="" class="object-cover w-full h-96" />
          </div>
          <h2 class="text-sm">{{ insta.usuario }}</h2>
        </div>
      </div>
      <div class="px-3 mx-auto py-4 grid grid-cols-10 gap-x-2">
        <div class="flex gap-x-4 col-span-8">
          <NotificationsChange />
          <Comment fill="white" />
        </div>
        <div class="col-span-2 items-center grid justify-end">
          <Save fill="white" />
        </div>
        <p class="text-white col-span-10 font-bold pt-2 capitalize text-sm">{{ insta.likes }} Me gusta</p>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
