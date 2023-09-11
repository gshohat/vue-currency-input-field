<script setup>
const props = defineProps(['options']);
const emit = defineEmits(['valueChange']);

function handleOnChange(event) {
  const value = event.target.value;

  const regex = new RegExp(`[${props.options.currency},]`);
  const valueWithoutSpecialChars = value.split(regex).join('');
  const num = parseInt(valueWithoutSpecialChars);

  let currencyRegexStr;
  props.options.currency === '$' ?
      currencyRegexStr = `\\${props.options.currency}` :
      currencyRegexStr = props.options.currency;
  const currencyRegex = new RegExp(currencyRegexStr);
  if (!value.match(currencyRegex))
    event.target.value = `${props.options.currency}${event.target.value}`;
  else if (num > 999) {
    event.target.value = `${props.options.currency}${addComma(valueWithoutSpecialChars)}`;
  }
  emit('valueChange', event.target.value);
}

function addComma(str) {
  if (str.length < 4)
    return str;
  const prefixComma = addComma(str.slice(0, str.length - 3));
  const suffixComma = str.slice(str.length - 3, str.length);
  return `${prefixComma},${suffixComma}`;
}

</script>

<template>
  <input
      type="text"
      name="money"
      :placeholder="options.placeHolder"
      @input="handleOnChange"
  />

</template>

<style scoped>

</style>
