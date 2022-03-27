# Vue3-clickoutside-component

> A simple Vue3 directive for clicking outside component.
## Install

```bash
npm install --save vue3-clickoutside-component
```


## How to use it ?

```js
import { createApp } from 'vue'
import App from './App.vue'
import clickOutside from 'vue3-clickoutside-component'
const app = createApp(App)

app.use(clickOutside)
```

```js
<template>
  <div class="dropdown" v-click-outside="() => hideDropdown()"></div>
</template>
<script setup>
  function hideDropdown() {
    console.log("close dropdown")
  }
</script>

### OR 

<script>
  methods: {
    hideDropdown() {
      console.log("close dropdown")
    }
  }
</script>
```


## License

[MIT](http://opensource.org/licenses/MIT)
