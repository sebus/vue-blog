<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  gender: String,
  pet: Object,
})
</script>

<template>
  <p>
    At home, {{ gender === 'male' ? 'his' : 'her' }} lively compagnion is {{ pet.name }} a
    {{ pet.age }}-year-old {{ pet.species }}.
  </p>
</template>

<style scoped></style>
