<template>
    <div class='header'>
        <router-link to="/">
            <div class='header-back iconfont icon-zuo'></div>
        </router-link>
        
        <div class='header-title'>城市页面选择</div>
    </div>
</template>
<script>
export default {
    name:'CityHeader',
    data(){
        return{

        }
    }
}
</script>
<style scoped>
    .header{
        background-color: #00bcd4;
        color:snow;
        height: .86rem;
    }
    .header-back{
        float:left;
        line-height: .86rem;
        margin-left:.2rem;
        color:snow;
    }
    .header-title{
        line-height: .86rem;
        text-align: center;
    }

</style>