<template>
    <div class="weekend">
        <div class='weekend-header'>周末精选</div>
        <div class='weekend-content'>
            <div class="weekend-item" v-for="(item,index) in weekendList" :key='index'>
                <img :src="item.imgSrc" class="weekend-img">
                <div class="weekend-title">{{item.title}}</div>
                <div class='weekend-sale'>{{item.sale}}</div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'WeekendHome',
    data(){
        return{
            weekendList:[
                {
                    id:'001',
                    imgSrc:"//imgs.qunarzz.com/vs_ceph_b2c_001/1a1bd0da-5b12-43a4-90ce-d6ee270b256d.jpg_r_480x320x95_fe9a7cb6.jpg",
                    title:'北京-石门 5日游',
                    sale:'$3080'
                },
                {
                    id:'002',
                    imgSrc:"//imgs.qunarzz.com/vs_ceph_b2c_001/1a1bd0da-5b12-43a4-90ce-d6ee270b256d.jpg_r_480x320x95_fe9a7cb6.jpg",
                    title:'北京-石门 5日游',
                    sale:'$3080'
                },
                {
                    id:'003',
                    imgSrc:"//imgs.qunarzz.com/vs_ceph_b2c_001/1a1bd0da-5b12-43a4-90ce-d6ee270b256d.jpg_r_480x320x95_fe9a7cb6.jpg",
                    title:'北京-石门 5日游',
                    sale:'$3080'
                },
                {
                    id:'004',
                    imgSrc:"//imgs.qunarzz.com/vs_ceph_b2c_001/1a1bd0da-5b12-43a4-90ce-d6ee270b256d.jpg_r_480x320x95_fe9a7cb6.jpg",
                    title:'北京-石门 5日游',
                    sale:'$3080'
                }
            ]
        }
    }
}
</script>
<style scoped>
.weekend-header{
    padding:.2rem .2rem;
    background-color: rgb(198, 202, 202);
}
.weekend-content{
    overflow: hidden;
    height: 0;
    padding-bottom: 320%;
}
.weekend-item{
    overflow: hidden;
    height: 0;
    padding-bottom:80%;
}
.weekend-img{
    width: 90%;
    display: block;
    margin:.2rem auto;
}
.weekend-title{
    text-align: center;
}
.weekend-sale{
    margin-top:.1rem;
    color: peru;
    font-weight: bolder;
    text-align: center;
}
</style>