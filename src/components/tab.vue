<template>
    <div class="tab">
        <div class="table-group">
            <div class="table-header" v-for="titler in Object.keys(list[0])" :key="titler">
                {{titler}}
            <ul class="table-row" v-for="item in list" :key="item">
                <li>{{item[titler]}}</li>
            </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'tab',
  props: ['list'],
  setup () {
    return { }
  }
}
</script>

<style scoped lang="scss">
ul {
    list-style:none;
}
.tab{
    display:table;
    white-space:nowrap;
    user-select:none;
    overflow:scroll;
    & .table-header{
        display:inline-block;
        padding:10px 0;
        text-align:center;
        & .table-row{
            display:block;
            padding:7px 17px;
            border-bottom:1px solid rgb(16, 121, 241);
        }
         & .table-row:nth-child(1){
             margin-top:7px;
            border-top:1px solid rgb(16, 121, 241);
        }
    }
}
</style>
