<script setup>
const props = defineProps({
  name: String,
  counter: {
    type: Number,
    required: false,
  },
});
</script>

<template>
  <h1>{{ name }}: {{ counter }}</h1>
</template>
