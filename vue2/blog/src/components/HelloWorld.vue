<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
    <h1 class="green">{{ msg }}</h1>
</template>

<style scoped>
  h1{
    color: orange;
  }
</style>


