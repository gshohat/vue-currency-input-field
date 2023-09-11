# Vue Currency Input Field

![NPM License](https://img.shields.io/npm/l/vue-currency-input-field)

**Lightweight** currency input component for [Vue](https://vuejs.org/) **< 5k** 😎 <br>
Emits the formatted value to parent component

## Usage

`npm i vue-currency-input-field`

```
<script setup>
import CurrencyInputField from 'vue-currency-input-field';

const options = {
  currency: '$',
  placeHolder: 'Please enter a number',
};

function handleValueChange(value) {
  //todo value '$123,456'
}
</script>


<template>
<CurrencyInputField :options="options" @value-change="handleValueChange"/>
</template
```


## Contact
Feel free to ping me 💫
<br>
connect@giladshohat.com

[giladshohat.com](https://giladshohat.com)
