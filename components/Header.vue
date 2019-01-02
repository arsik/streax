<template lang="pug">
  header.header
    .container
      .logo
        nuxt-link(to='/')
          Logo
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
  import Logo from '~/assets/svg/logo.svg'
  Vue.use(Antd)

  export default {
    components: {
      Logo
    }
  }
</script>

<style lang="stylus" scoped>
  .header
    width 100%
    height 8rem
    // padding 0 2rem
    background #fff

    .container
      display flex
      justify-content space-between
      align-items center

    .logo
      a 
        display block
        width 12rem
        height 2.4rem
        color black
        font-size 2rem

    .nav
      a
        & + a
          margin 0 0 0 2rem
</style>
