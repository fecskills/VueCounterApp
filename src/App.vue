<template>
  <main>
    <div>
      <h4>The current count is ...</h4>
      <h1>{{ count }}</h1>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
    </div>
  </main>
</template>
<script setup>
import { ref } from 'vue'

const count = ref(0);

</script>
<style scoped>
main {
  width: 100vw;
  height: 100vh;
  background-color: antiquewhite;
  display: flex;
  align-items: center;
  justify-content: center;
} 

div {
    text-align: center;
}

button {
    margin: 10px;
    padding: 10px;
    border-radius: 5px;
    /* border: none; */
    background-color: #1260bd;
    cursor: pointer;
    color: white;
    width: 5pc;
    font-size: 20px;
}

h1 {
    font-size: 72px;
    font-weight: 800;
    margin-bottom: 0px;
    margin-top: 0px;
}

button:hover {
    background-color: #03214e;
}
</style>