<template>
    <div>
        <header-home/>
        <swiper-home/>
        <icons-home/>
        <recommend-home/>
        <weekend-home/>
        <router-link to='/city'>
        <div>跳转到城市页面</div>
        </router-link>
    </div>
</template>
<script>
import header from './components/header'
import swiper from './components/swiper'
import icons from './components/icons'
import recommend from './components/recommend'
import weekend from './components/weekend'
export default{
    name:'Home',
    components:{
        "header-home":header,
        'swiper-home':swiper,
        'icons-home':icons,
        'recommend-home':recommend,
        'weekend-home':weekend
    },
    data(){
        return{
            
        }
    } 
}
</script>
