<template>
    <span class="btn" >{{content}}</span>
</template>

<script>
export default {
  name: 'btn',
  props: ['content'],
  setup () {
    return { }
  }
}
</script>

<style scoped lang="scss">
.btn {
  display:inline-block;
  padding:5px 17px;
  height:33px;
  line-height:33px;
  border-radius:3px;
  background:rgb(16, 121, 241);
  color:#fff;
}
</style>
