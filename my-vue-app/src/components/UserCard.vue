<template>
  <div class="card">
    <h3>{{ name }}</h3>
    <p>{{ role }}</p>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  role: String
});
</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  padding: 16px;
  width: 220px;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

h3 {
  margin: 0;
  color: #28d811;
}

p {
  margin-top: 8px;
  color: #eeff06;
}
</style>
