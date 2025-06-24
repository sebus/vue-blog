<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  gender: String,
  age: Number,
  job: String,
})
</script>

<template>
  <p>{{ gender === 'male' ? 'He' : 'She' }} a {{ age }}-year-old {{ job }}.</p>
</template>

<style scoped>
h1 {
  font-size: 24px;
  font-weight: bold;
}
</style>
