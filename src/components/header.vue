<template>
    <div class="header">
        <ul>
            <li><a href="#">首页</a></li>
            <li><a href="#" class="focus">学生管理</a></li>
            <li><a href="#">教师管理</a></li>
            <li><a href="#">留言管理</a></li>
            <li><a href="#">轮播图</a></li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'header'
}
</script>

<style scoped lang="scss">
.header{
    width:100vw;
    height:53px;
    background-color:#fff;
    box-shadow:2px 2px 2px rgb(247, 246, 246);
    & ul{
        list-style:none;
        text-align:center;
        line-height:53px;
        & li{
            display: inline-block;
            margin:0 15px;
            padding:0 10px;
            & a{
                text-decoration:none;
                color:black;
            }
        }
        & .focus{
            color:blue;
            &::after{
            display:block;
            content:'';
            width:100%;
            transform:translateY(-100%);
            color:blue;
            border-bottom:2px solid blue;
        }
        }
    }
}

</style>
