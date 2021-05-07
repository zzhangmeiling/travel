<template>
    <div class='recommend'>
        <div class='recommend-header'>热门推荐</div>
        <div class='recommend-content '>
            <div class="recommend-item border" v-for="(item,index) in recommendList" :key='index'>  
               <img class='recommend-img' :src="item.imgSrc">
               <div class='recommend-text'>{{item.title}}</div>
               <div class='recommend-sale'>{{item.sale}}</div>
            </div>
            
            
        </div>
    </div>
</template>

<script>
export default {
    name:'Recommend-Home',
    data(){
        return{
            recommendList:[
                {
                    id:'001',
                    imgSrc:"//img1.qunarzz.com/sight/p0/201405/12/51b63883c25f5d87af3c08bb016e2bd7.jpg_256x160_2c506073.jpg",
                    title:"恭王府",
                    sale:'￥42.5'
                },
                {
                    id:'001',
                    imgSrc:"//img1.qunarzz.com/sight/p0/201405/12/51b63883c25f5d87af3c08bb016e2bd7.jpg_256x160_2c506073.jpg",
                    title:"恭王府",
                    sale:'￥42.5'
                },
                {
                    id:'001',
                    imgSrc:"//img1.qunarzz.com/sight/p0/201405/12/51b63883c25f5d87af3c08bb016e2bd7.jpg_256x160_2c506073.jpg",
                    title:"恭王府",
                    sale:'￥42.5'
                },
                {
                    id:'001',
                    imgSrc:"//img1.qunarzz.com/sight/p0/201405/12/51b63883c25f5d87af3c08bb016e2bd7.jpg_256x160_2c506073.jpg",
                    title:"恭王府",
                    sale:'￥42.5'
                }
            ]
        }
    }
}
</script>
<style scoped>
    .recommend-header{
        background-color: rgb(217, 222, 223);
        padding: .2rem .2rem;
    }
    .recommend-content{
        overflow: hidden;
        height: 0;
        padding-bottom: 85%;

    }
    .recommend-item{
        overflow: hidden;
        height: 0;
        width: 50%;
        padding-bottom: 42%;
        float: left;
    }
    .recommend-img{
        display: block;
        width: 90%;
        margin:.1rem auto;
    }
    .recommend-text{
        text-align: center;
        margin-top:.1rem;
    }
    .recommend-sale{
        text-align: center;
        color: orange;
        font-size:.32rem;
        font-weight: bolder;
        margin-top:.1rem;
    }
</style>