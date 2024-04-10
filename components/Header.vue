<template>
  <header class="bg-black py-4 border-blue-50/10 border-b-[0.1px] fixed w-full z-50">
    <div class="mx-auto w-5/6 grid grid-cols-12 items-center justify-center gap-x-4">
      <div class="bg-[#262626] items-center rounded-md p-1 col-span-12 xs:col-span-11 grid grid-cols-12">
        <span
          class="pi pi-search text-center col-span-1 bg-transparent"
          style="font-size: 0.8rem; color: #a8a8a8"></span>
        <input
          class="w-full placeholder:text-sm col-span-8 placeholder:text-[#a8a8a8] bg-transparent focus:outline-none focus:ring-0 focus:border-transparent text-white pl-2"
          type="text"
          placeholder="Buscar" />
      </div>
      <div class="hidden xs:grid xs:grid-cols-1">
        <span class="pi pi-heart" style="font-size: 1rem; color: white"></span>
      </div>
    </div>
  </header>
</template>

<script setup>
import "primeicons/primeicons.css";
</script>
