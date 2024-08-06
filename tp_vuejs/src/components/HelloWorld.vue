<template>
  <div class="hello">
    <h1>Hello World </h1>
    <p>{{ props.user.name }} {{ props.user.age }}</p>
  </div>
</template>

<script setup>
 const props = defineProps(['user']);
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>
