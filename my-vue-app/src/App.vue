<!-- <template><h1>Hello SPEC Developers</h1>
<ol>
  <li v-for="lang in ['JS','Python','Go']" :key="lang">
    {{ lang }}
  </li>
</ol>

</template> -->

<template>
  <div class="container">
    <h2>Greeting App</h2>

    <input type="text" v-model="name" placeholder="Enter your name" />

    <!-- Greeting appears only when name is not empty -->
    <p v-if="name.trim()">Hello, {{ name }} 👋</p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const name = ref("");
</script>

<style>
.container {
  font-family: Arial, sans-serif;
  padding: 40px;
}

input {
  padding: 8px;
  font-size: 16px;
}

p {
  margin-top: 15px;
  font-size: 20px;
  color: green;
}
</style>
