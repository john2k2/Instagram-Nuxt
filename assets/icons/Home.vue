<script setup>
defineProps({
  fill: {
    type: String,
    default: "white",
  },
  stroke: {
    type: String,
    default: "none",
  },
});
</script>

<template>
  <div>
    <svg
      xmlns="http://www.w3.org/2000/svg"
      aria-label="Inicio"
      class="x1lliihq x1n2onr6 x5n08af"
      :fill="fill"
      :stroke="stroke"
      height="24"
      role="img"
      viewBox="0 0 24 24"
      width="24">
      <title>Inicio</title>
      <path
        d="M22 23h-6.001a1 1 0 0 1-1-1v-5.455a2.997 2.997 0 1 0-5.993 0V22a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V11.543a1.002 1.002 0 0 1 .31-.724l10-9.543a1.001 1.001 0 0 1 1.38 0l10 9.543a1.002 1.002 0 0 1 .31.724V22a1 1 0 0 1-1 1Z" />
    </svg>
  </div>
</template>

<style scoped></style>
