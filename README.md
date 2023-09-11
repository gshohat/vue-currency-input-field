# Vue Currency Input Field

![NPM License](https://img.shields.io/npm/l/vue-currency-input-field)

**Lightweight** currency input component for [Vue](https://vuejs.org/) **< 5k** 😎 <br>
Emits the formatted value to parent component

![currency-input-field](https://github.com/gshohat/vue-currency-input-field/assets/91323932/891147a4-7b4b-4b3d-ab56-e6fc76bda3d6)

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
