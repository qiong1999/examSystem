<template>
    <div class="tab">
        <div v-for="item in list" :key="item">
            <span v-for="itt in item" :key="itt">
                {{itt}}
            </span>
        </div>
    </div>
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

<style scoped lang="scss">
.tab{
    display:inline-block;
    & div{
        height:47px;
        line-height:47px;
        border-bottom:1px solid rgb(230, 230, 230);
        & span{
            padding:0 20px;
            background:red;
            border:1px solid #fff;
        }
    }
}
</style>
