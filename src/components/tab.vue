<template>
    <div>hello</div>
</template>

<script>
export default {
  name: 'tab',
  setup () {
    const list = [
      { stuId: '1714010302', username: '梁薪驰', password: '123456', photo: 'null', root: true },
      { stuId: '1714010812', username: '驰子', password: '123456', photo: 'null', root: true }
    ]
    return { list }
  }
}
</script>

<style scoped>

</style>
