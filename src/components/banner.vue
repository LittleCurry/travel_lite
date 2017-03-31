<template>
    <div>
        <div class="page-cover"
                v-if="show&&fixHead"
                @click="showMenus">
        </div>
        <img src="../assets/images/logo.png">
        <p>你好你好你好</p>



        <nv-menu :show-menu="show"
            :page-type="pageType"
            :nick-name="nickname"
            :profile-url="profileimgurl"
            v-if="fixHead" ></nv-menu>
    </div>
</template>

<script>
    export default {
        replace: true,
        components: {
            'nvMenu': require('./menu.vue')
        }
    };
</script>