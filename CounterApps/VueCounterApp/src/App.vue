<script setup>
import { ref } from "vue"
const count = ref(0)

const addToCount = () => {
  console.log("Hello from add to count")
  count.value = count.value + 1
}
const subtractFromCount = () => {
  console.log("Hello from subtract from count")
  count.value = count.value - 1
}
</script>

<script>
</script>
<template>
  <main>
    <div>
      <h4>The current count is...</h4>
      <h1>{{ count }}</h1>
      <button @click="subtractFromCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  text-align: center;
}
</style>