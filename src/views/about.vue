<template>
    <div style="height: 100%;">
        <nv-head page-type="关于" :fix-head="true" :need-add="true" ></nv-head>
        
        <dl class="about-info">

            <dt>关于项目</dt>
            <dd>a_vuedemo是一个主要针对有旅行需求, 但是没有足够预算的人群, 想要通过以兼职的形式来赚取旅行费用的平台</dd>
        
            <dt>源码地址</dt>
            
            <dd>
                <a href="https://github.com/LittleCurry/travel_lite">
                    https://github.com/LittleCurry/travel_lite</a>
            </dd>
            
            <dt>意见反馈</dt>
            <dd>
                <a href="https://github.com/LittleCurry/travel_lite/issues">
                    发表意见或者提需求</a>
            </dd>
            
            <dt>当前版本</dt>
            <dd>V 2.0</dd>

        </dl>
    </div>
</template>
<script>
    import nvHead from '../components/header.vue';
    export default {
        components: {
            nvHead
        }
    };
</script>