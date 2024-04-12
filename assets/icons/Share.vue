<script setup>
defineProps({
  fill: {
    type: String,
    default: "white",
  },
});
</script>

<template>
  <div>
    <svg
      xmlns="http://www.w3.org/2000/svg"
      aria-label="Compartir publicación"
      class="x1lliihq x1n2onr6 x1roi4f4"
      :fill="fill"
      height="24"
      role="img"
      viewBox="0 0 24 24"
      width="24">
      <title>Compartir publicación</title>
      <line fill="none" :stroke="fill" stroke-linejoin="round" stroke-width="2" x1="22" x2="9.218" y1="3" y2="10.083" />
      <polygon
        fill="none"
        points="11.698 20.334 22 3.001 2 3.001 9.218 10.084 11.698 20.334"
        :stroke="fill"
        stroke-linejoin="round"
        stroke-width="2" />
    </svg>
  </div>
</template>

<style scoped></style>
