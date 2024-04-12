<script setup>
defineProps({
  fill: {
    type: String,
    default: "white",
  },
});

const like = ref(true);

const likes = () => {
  like.value = !like.value;
};
</script>

<template>
  <div @click="likes">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      aria-label="Guardar"
      class="x1lliihq x1n2onr6 x5n08af"
      :fill="fill"
      height="24"
      role="img"
      viewBox="0 0 24 24"
      width="24">
      <title>Guardar</title>
      <polygon
        :fill="like ? 'none' : 'white'"
        points="20 21 12 13.44 4 21 4 3 20 3 20 21"
        :stroke="fill"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2" />
    </svg>
  </div>
</template>
