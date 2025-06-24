<script setup>
import CardTitle from './CardTitle.vue'
import FirstParagraph from './FirstParagraph.vue'
import SecondParagraph from './SecondParagraph.vue'
import ThirdParagraph from './ThirdParagraph.vue'

const props = defineProps({
  personList: {
    type: Object,
    required: true,
  },
})

console.log(props.personList)
</script>

<template>
  <section>
    <CardTitle
      :firstname="personList.firstname"
      :lastname="personList.lastname"
      :gender="personList.gender"
    />
    <FirstParagraph :gender="personList.gender" :age="personList.age" :job="personList.job" />
    <SecondParagraph :firstname="personList.firstname" :hobbies="personList.hobbies" />
    <ThirdParagraph :gender="personList.gender" :pet="personList.pet" />
    <font-awesome-icon :icon="['fas', 'heart']" />
  </section>
</template>

<style scoped>
section {
  padding: 20px;
  border-radius: 15px;

  box-shadow: 0 0 7px v-bind('personList.favoriteColor');

  margin: 20px 0;
}
</style>
