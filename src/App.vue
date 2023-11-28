<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import Greet from './components/Greet.vue'
import Person from './components/Person.vue'

  const person = {
    name: "oleg",
    email: "electrochange@mail.ru",
    age:36
  }
</script>

<template>
  

  <main>
    <Greet name="Oleg Podzorov"/>
    <Greet name="Someone" />
    <Person :person="person" />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

</style>
