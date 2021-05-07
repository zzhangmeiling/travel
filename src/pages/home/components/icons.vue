<template>
    <div class='icons'>
        <div class='icons-item' v-for="(item,index) in iconsList" :key='index'>
            <img class='icons-img' :src="item.imgSrc">
            <div class='icons-text'>{{item.text}}</div>
        </div>
       
    </div>
</template>
<script>
export default {
    name:'IconsHome',
    data(){
        return {
            iconsList:[
                {
                    id:'001',
                    imgSrc:"//s.qunarzz.com/homenode/images/touchheader/hotel.png",
                    text:'酒店'
                },
                {
                    id:'002',
                    imgSrc:"//s.qunarzz.com/homenode/images/touchheader/flight.png",
                    text:'机票'
                },
                {
                    id:'003',
                    imgSrc:"//s.qunarzz.com/homenode/images/touchheader/train.png",
                    text:'火车票'
                },
                {
                    id:'004',
                    imgSrc:"//s.qunarzz.com/homenode/images/touchheader/package.png",
                    text:'度假'
                },
                {
                    id:'005',
                    imgSrc:"https://picbed.qunarzz.com/f5e5770393d759578962e53ee67798c8.png",
                    text:'海外酒店'
                },
                {
                    id:'006',
                    imgSrc:"https://picbed.qunarzz.com/a36d2288f19e54562338f4d8ef986288.png",
                    text:'低价机票'
                },
                {
                    id:'007',
                    imgSrc:"https://picbed.qunarzz.com/377db8cb2143aebf01869c9baad3d325.png",
                    text:'低价船票'
                },
                {
                    id:"008",
                    imgSrc:"https://picbed.qunarzz.com/ae617a31e0bd5803d76918b817f6d942.png",
                    text:"自由行"
                }
            ]
        }
    }
}
</script>
<style scoped>
    .icons{
        overflow: hidden;
        height: 0;
        padding-bottom:50%;
    }
    .icons-item{
        overflow: hidden;
        height: 0;
        width:25%;
        padding-bottom: 25%;
        float:left;
    }
    .icons-img{
        display: block;
        width:60%;
        margin:.2rem auto;
    }
    .icons-text{
        text-align: center;
        font-size: .32rem;
    }
</style>