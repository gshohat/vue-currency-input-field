# Vue Currency Input Field

![NPM License](https://img.shields.io/npm/l/vue-currency-input-field)

**Lightweight** currency input component for [Vue](https://vuejs.org/) **< 5k** 😎 <br>
Emits the formatted value to parent component

![currency-input-field](https://private-user-images.githubusercontent.com/91323932/266929316-c585ef19-b03d-45bd-ab65-b089ec3d8ef3.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE2OTQ0MTQ3MjQsIm5iZiI6MTY5NDQxNDQyNCwicGF0aCI6Ii85MTMyMzkzMi8yNjY5MjkzMTYtYzU4NWVmMTktYjAzZC00NWJkLWFiNjUtYjA4OWVjM2Q4ZWYzLmdpZj9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFJV05KWUFYNENTVkVINTNBJTJGMjAyMzA5MTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMwOTExVDA2NDAyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTRiOTZiNjIzMzBiYjhiOTlmMzM4MmJjMGU4YTA2MzlhZjM0NDM5Nzc1NTUwNmFkZGQ1MTZiZWMyYjVhOGIxNWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.v4AVM8aJR66w6HY5_zqNTkAVELnHkxfqfY1X9Sjnruw)

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
