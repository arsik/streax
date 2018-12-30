<template lang="pug">
  .container
    h1 Streax
    Button hello
</template>

<script>
// import Logo from '~/components/Logo.vue'
import Vue from 'vue'
import { Button } from 'ant-design-vue'

export default {
  components: {
    Button
  }
}
</script>

<style lang="stylus">
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
