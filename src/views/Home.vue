<template>
    <Header/>
    <Tab />
    <Btn content="批量导入"/>
</template>

<script>

import Header from '../components/header.vue'
import Btn from '../components/btn.vue'
import Tab from '../components/tab.vue'
export default {
  name: 'home',
  components: {
    Header,
    Btn,
    Tab
  }
}
</script>

<style scoped>

</style>
