<script setup>
import { useSupabaseAuth } from "@vueuse/supabase";

const supaAuth = useSupabaseAuth().auth;

const login = () => {
  supaAuth.signIn();
};

const { user } = supaAuth;
</script>

<template>
  <div class="w-full h-screen flex items-center justify-center">
    <UButton v-if="!user" @click="login" class="bg-blue-500 text-white px-4 py-2 rounded-md">Button</UButton>
  </div>
</template>

<style scoped></style>
