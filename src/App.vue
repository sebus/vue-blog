<script setup>
import Header from './components/Header.vue'
import CardDescription from './components/CardDescription.vue'
import Footer from './components/Footer.vue'

const personsList = [
  {
    gender: 'female',
    firstname: 'Emily',
    lastname: 'Parker',
    age: 24,
    job: 'teacher',
    hobbies: ['read books', 'go hiking'],
    pet: {
      name: 'Whiskers',
      age: 2,
      species: 'ferret',
    },
    favoriteColor: 'red',
  },
  {
    gender: 'male',
    firstname: 'Marcus',
    lastname: 'Bennett',
    age: 38,
    job: 'architect',
    hobbies: ['watch bird', 'play chess'],
    pet: {
      name: 'Nala',
      age: 6,
      species: 'dog',
    },
    favoriteColor: 'blue',
  },
  {
    gender: 'female',
    firstname: 'Sophia',
    lastname: 'Rodriguez',
    age: 31,
    job: 'environmental scientist',
    hobbies: ['play guitar', 'bake cakes'],
    pet: {
      name: 'Paws',
      age: 3,
      species: 'cat',
    },
    favoriteColor: 'orange',
  },
  {
    gender: 'male',
    firstname: 'Oliver',
    lastname: 'Hughes',
    age: 56,
    job: 'carpenter',
    hobbies: ['paint', 'ride horses'],
    pet: {
      name: 'Bubble',
      age: 4,
      species: 'snake',
    },
    favoriteColor: 'purple',
  },
]
</script>

<template>
  <Header />

  <div class="content container">
    <CardDescription v-bind:personList="personsList[0]" />
    <CardDescription v-bind:personList="personsList[1]" />
    <CardDescription v-bind:personList="personsList[2]" />
    <CardDescription v-bind:personList="personsList[3]" />
  </div>

  <Footer />
</template>

<style scoped></style>
