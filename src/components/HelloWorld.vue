<script setup>
import { reactive, ref } from 'vue'

const count = ref(0)
const person = reactive({
  name: 'John',
  age: 30
})

function increment() {
  count.value++
  console.log(count)
  console.log(person)
}
</script>

<template>
  <p>
    <div>{{ count }}</div>
    <button @click="increment()">
      增加
    </button>
  </p>
</template>

<style scoped>
</style>
