<template>
    <div style="height: 100%;">
        <nv-head page-type="需求"
                 :fix-head="true"
                 :need-add="true"></nv-head>
    <router-link :to="{name:'submitNeed'}">
        <el-button style="margin-top: 100px; margin-left: 50px;" type="primary" @click.native="makeNeed">发布<i class="el-icon-upload el-icon--right"></i></el-button>
    </router-link>
    </div>
</template>

<script>
import nvHead from '../components/header.vue';

export default {
    methods: {
        makeNeed() {
            // console.log('你好');
            this.$router.push('/about.vue');
        }
    },
    components: {
        nvHead
    }
};

</script>

<style>
.el_button {
    margin-top: 100px;
    background-color: orange;
}

.el-carousel__item p {
    height: 50px;
    width: 100%;
    color: white;
    background-color: rgba(0,0,0,0.5);
    bottom: 0;
    padding-top: 17px;
    padding-right: 10px;
    font-size: 17px;
    text-align: right;
    position: absolute;
    bottom: 0;
}
</style>