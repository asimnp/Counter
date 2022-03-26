<script setup>
const props = defineProps({
  name: String,
});

const emit = defineEmits(["increment", "decrement", "reset"]);

function handleClick(e) {
  const value = e.target.value;

  if (value === "increment") {
    emit("increment");
  } else if (value === "decrement") {
    emit("decrement");
  } else if (value === "reset") {
    emit("reset");
  }
}
</script>

<template>
  <button @click="handleClick" value="increment">{{ name }}</button>
</template>
