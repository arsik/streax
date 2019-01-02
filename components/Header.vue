<template lang="pug">
  header.header
    .container
      .logo
        nuxt-link(to='/') Streax
      nav.nav
        nuxt-link(to='/') Проекты
        nuxt-link(to='/') Как это работает?
      .profile
        a-dropdown-button
          | annex
          a-menu(slot='overlay')
            a-menu-item(key='1')
              a-icon(type='user') 
              | Профиль
            a-menu-item(key='2')
              a-icon(type='user') 
              | Настройки
            a-menu-item(key='3')
              a-icon(type='user') 
              | Выйти

</template>

<script>
  import Vue from 'vue'
  import Antd from 'ant-design-vue'
  Vue.use(Antd)

  export default {

  }
</script>

<style lang="stylus" scoped>
  .header
    width 100%
    height 6rem
    // padding 0 2rem
    background #f0f0f0

    .container
      display flex
      justify-content space-between
      align-items center

    .logo
      a 
        color black
        font-size 2rem

    .nav
      a
        & + a
          margin 0 0 0 2rem
</style>
