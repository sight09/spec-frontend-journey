<!-- DAY 1 -->

<!-- <template><h1>Hello SPEC Developers</h1>
<ol>
  <li v-for="lang in ['JS','Python','Go']" :key="lang">
    {{ lang }}
  </li>
</ol>

</template> -->

<!-- END OF DAY 1 -->




<!-- DAY 2 -->

<!-- <template>
  <div class="container">
    <h2>Greeting App</h2>

    <input
      type="text"
      v-model="name"
      placeholder="Enter your name"
    />

    <!-- Greeting appears only when name is not empty -->
    <!-- <p v-if="name.trim()">
      Hello, {{ name }} 👋
    </p>
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
</style> --> 

<!-- END OF DAY 2 -->





<!-- DAY 3 -->

<!-- <template>
  <!-- <div class="container">
    <h2>User Cards</h2>

    <div class="cards">
      <UserCard name="Amanuel Alemu" role="Frontend Developer" />
      <UserCard name="Sara Tesfaye" role="UI/UX Designer" />
      <UserCard name="Daniel Bekele" role="Backend Engineer" />
    </div>
  </div>
</template>

<script setup>
import UserCard from "./components/UserCard.vue";
</script>

<style>
.container {
  padding: 40px;
  font-family: Arial, sans-serif;
}

.cards {
  display: flex;
  gap: 20px;
}
</style> --> -->

<!-- END OF DAY 3 -->







<!-- DAY 4 -->

<template>
  <div class="counter-app">
    <h2>Counter App</h2>

    <!-- Show the count -->
    <h1>{{ count }}</h1>

    <!-- Buttons with event handlers -->
    <button 
      @click="decrease" 
      :disabled="count === 0"
    >
      –
    </button>

    <button @click="increase">
      +
    </button>
  </div>
</template>

<script setup>
import { ref } from "vue";

// reactive state (ref)
const count = ref(0);

// method handlers
function increase() {
  count.value++;
}

function decrease() {
  if (count.value > 0) {
    count.value--;
  }
}
</script>

<style>
.counter-app {
  font-family: Arial, sans-serif;
  text-align: center;
  padding: 40px;
}

h1 {
  font-size: 48px;
  margin: 20px 0;
}

button {
  font-size: 24px;
  margin: 0 10px;
  padding: 10px 20px;
  cursor: pointer;
}

button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}
</style>

