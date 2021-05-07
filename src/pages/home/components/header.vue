<template>
    <div class='header'>
        <div class="left iconfont icon-zuo"></div>
        <div class="content"><span class='iconfont icon-chazhao'></span>
        请输入城市|景点</div>
        <div class="right">城市<span class='iconfont icon-xiangxia'></span></div>
    </div>
</template>
<script>
export default {
    name:'HomeHeader',
    data(){
        return{
        }
    }
}
</script>
<style  scoped>
    .header{
        background-color :#00bcd4;
        height: .8rem;
        width :100%;
        display: flex;
        align-items: center;
        font-size:.32rem;
    }
    .header .left{
        float:left;
        color:#fff;
        margin:0 .3rem;
    }
    .header .content{
        flex:1;
        background: snow;
        border-radius: .2rem;
        height: .65rem;
        color:#666;
        text-align: center;
        line-height: .65rem;
    }
    .header .right{
        float: right;
        color:#fff;
        margin:0 .3rem;
    }
    .icon-xiangxia{
        margin-left:.1rem;
    }
</style>