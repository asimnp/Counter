<script setup>
import { ref } from "vue";

import H1Title from "./components/H1Title.vue";
import Button from "./components/Button.vue";

const counter = ref(0);
</script>

<template>
  <H1Title name="Counter" :counter="counter" />
  <Button name="Increment" value="increment" @increment="counter++" />
  <Button name="Decrement" value="decrement" @decrement="counter--" />
  <Button name="Reset" value="reset" @reset="counter = 0" />
</template>

<style></style>
