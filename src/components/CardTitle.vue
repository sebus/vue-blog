<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  firstname: String,
  lastname: String,
  gender: String,
})
</script>

<template>
  <img src="../assets/img/emily-parker.jpg" />
  <h1
    :class="{
      isFemale: gender === 'female',
    }"
  >
    {{ firstname }} {{ lastname }}
  </h1>
</template>

<style scoped>
h1 {
  font-size: 24px;
  font-weight: bold;
}
img {
  width: 100%;
  /* Détermine la hauteur automatiquement de manière à respecter le ratio donné */
  aspect-ratio: 16/10;
  object-fit: cover;
  object-position: top;
  border-radius: 5px;
}
.isFemale {
  color: orange;
}
</style>
