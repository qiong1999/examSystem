<template>
    <Header/>
    <search />
    <Btn content="批量导入"/>
    <Tab  :list = "list" />
</template>

<script>

import Header from '../components/header.vue'
import Btn from '../components/btn.vue'
import Tab from '../components/tab.vue'
import Search from '../components/search.vue'
export default {
  name: 'home',
  components: {
    Header,
    Btn,
    Tab,
    Search
  },
  setup () {
    const list = [
      { stuId: '1714010812', username: '驰子', password: '123456', photo: 'null', root: true },
      { stuId: '1714010812', username: '欧阳驰子', password: '123456', photo: 'null', root: true }
    ]
    return { list }
  }
}
</script>

<style scoped>

</style>
