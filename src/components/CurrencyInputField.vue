<script setup>
const props = defineProps(['options']);

function handleOnChange(event) {
  const value = event.target.value;
  const dollarChar = /\$/;
  if (!value.match(dollarChar))
    event.target.value = `$${event.target.value}`;

}

</script>


<template>
  <input
      type="text"
      name="money"
      placeholder="Please enter a $ amount"
      @input="handleOnChange"
  />

</template>

<style scoped>

</style>
