<template>
    <div class='search'>
        <input class='search-input' type="text"  placeholder="请输入城市名称"/>
    </div>
</template>
<script>
export default {
    name:'CitySearch',
    data(){
        return{

        }
    }
}
</script>
<style scoped>
    .search{
        height: .72rem;
        background-color: #00bcd4;
        padding:0 .1rem;
    }
    .search-input{
        border-radius: .1rem;
        width: 100%;
        box-sizing: border-box;
        text-align: center;
        height: .62rem;
        line-height: .6rem;
    }
    
</style>