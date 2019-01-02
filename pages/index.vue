<template lang="pug">
  .wrapper
    Header
    .container
      a-row(:gutter="16")
        a-col(class="gutter-row" :span="6" v-for="(item, index) in cards" :key="index")
          a-card(:loading="true" title="Проект 1") whatever content
    Footer
</template>

<script>
import Vue from 'vue'
import Antd from 'ant-design-vue'
import Header from '~/components/Header'
import Footer from '~/components/Footer'
Vue.use(Antd)

export default {
  components: {
    Header,
    Footer
  },
  data: function () {
    return {
      cards: [
        {},
        {},
        {},
        {},
      ]
    }
  }
}
</script>

<style lang="stylus">


</style>
