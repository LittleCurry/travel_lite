<template>
    <div style="height: 100%;">
        <!--<nv-banner></nv-banner>-->
        <nv-head page-type="推荐"
                 :fix-head="true"
                 :need-add="true"></nv-head>
        <el-carousel :interval="3000" type="card" height="300px">
            <el-carousel-item v-for="item in 6">
                    <img mode="aspectFit" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1490941844441&di=8b1c1c77752e801d960c2945b9b4da93&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fwallpaper%2F5%2F553dc1e2be070.jpg">
                    <p>【邮轮游记攻略】彼岸的旅行箱之悠游加勒比</p>
            </el-carousel-item>
        </el-carousel>    
    </div>
</template>
<script>
import nvHead from '../components/header.vue';
import nvBaner from '../components/banner.vue';

export default {
    components: {
        nvHead,
        nvBaner
    }
};
</script>

<style>
.el-carousel__item {
    padding-top: 46px;
}
/*.el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
}
.el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
}*/
.el-carousel__item img {
    width: 100%;
    height: 100%;
}
.el-carousel__item p {
    height: 30px;
    color: white;
    background: red;
    padding-right: 20px;
    font-size: 17px;
    text-align: right;
    margin-top: -50px;
}
</style>