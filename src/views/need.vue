<template>
    <div style="height: 100%;">
        <nv-head page-type="需求"
                 :fix-head="true"
                 :need-add="true"></nv-head>

    <!--<router-link :to="{name:'submitNeed'}">-->
        <!--<el-button style="margin-top: 100px; margin-left: 50px;" type="primary" @click.native="makeNeed">我要发布<i class="el-icon-upload el-icon--right"></i></el-button>-->
        <!--<el-alert style="margin-top: 50px" title="我要发布" type="success" :closable="false"></el-alert>-->
    <!--</router-link>-->
    
    <el-table
    :data="tableData2"
    style="width: 100%; margin-top: 50px"
    :row-class-name="tableRowClassName">
    <el-table-column
      prop="date"
      label="日期"
      width="180">
    </el-table-column>
    <el-table-column
      prop="name"
      label="姓名"
      width="180">
    </el-table-column>
    <el-table-column
      prop="address"
      label="目的地">
    </el-table-column>
  </el-table>
  <router-link :to="{name:'submitNeed'}">
      <i  class="iconfont icon-top" style="height:20px width:20px">
          <div style="width:50px;
                      height:50px;
                      font-size:15px;
                      background-color: #ff6600; 
                      border-top-left-radius:25px;
                      border-top-right-radius:25px;
                      border-bottom-right-radius:25px;
                      border-bottom-left-radius:25px">
            <p style="font-size:15px; margin-left:10px; padding-top:10px">我要</p>
            <p style="font-size:15px; margin-left:10px">发布</p>
          </div>
      </i>
  </router-link>
    </div>

</template>

<script>
import nvHead from '../components/header.vue';

export default {
    methods: {
        makeNeed() {
            this.$router.push('/about.vue');
        },
        tableRowClassName(row, index) {
            if (index % 2 === 1) {
                return 'info-row';
            } else if (index % 2 === 0) {
                return 'positive-row';
            }
            return '';
        }
    },
    data() {
        return {
            tableData2: [{
                date: '2016-05-02',
                name: '张三',
                address: '丽江玉龙雪山、大研古城'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }, {
                date: '2016-05-04',
                name: '李四',
                address: '崖州三亚'
            }, {
                date: '2016-05-01',
                name: '王二狗',
                address: '安徽黄山'
            }, {
                date: '2016-05-03',
                name: '朱老六',
                address: '神奇九寨沟'
            }]
        };
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

.el-table .info-row {
    background: #c9e5f5;
  }

.el-table .positive-row {
    background: #e2f0e4;
  }
</style>