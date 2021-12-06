<template lang="pug">
#app
  Top
  #middle
    #left
      Menu
      Update
    #right
      Marquee
      Content
    Footer
</template>

<script>
// 引用自己的元件
import Top from './components/Top.vue'
import Menu from './components/Menu.vue'
import Update from './components/Update.vue'
import Marquee from './components/Marquee.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  // 飲用後註冊元件
  components: {
    Top,
    Menu,
    Update,
    Marquee,
    Content,
    Footer
  }
}
</script>
