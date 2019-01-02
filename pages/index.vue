<template lang="pug">
  .wrapper
    Header
    .container
      .ant-row
        .ant-col-8
          h1 Streax
          a-switch(defaultChecked)
</template>

<script>
import Vue from 'vue'
import Antd from 'ant-design-vue'
import Header from '~/components/Header'
Vue.use(Antd)

export default {
  components: {
    Header
  }
}
</script>

<style lang="stylus">


</style>
