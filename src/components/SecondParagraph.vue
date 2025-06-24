<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  firstname: String,
  hobbies: Object,
})
</script>

<template>
  <p>Outside of work, {{ firstname }} likes to {{ hobbies[0] }} and {{ hobbies[1] }}.</p>
</template>

<style scoped>
h1 {
  font-size: 24px;
  font-weight: bold;
}
</style>
