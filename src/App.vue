<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import Greet from './components/Greet.vue'
import Person from './components/Person.vue'

  const person = {
    name: "oleg",
    email: "oleg@mail.ru",
    age:35
  }
</script>

<template>
  

  <main>
    <Greet name="Oleg"/>
    <Person :person="person" />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

</style>
