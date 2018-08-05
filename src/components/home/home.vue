<template>
  <el-container class="home">
    <el-header height="auto">
      <el-card class="box-card">
        <div slot="header" class="div-header clearfix">
          <span>地区选择</span>
        </div>
        <div v-for="o in 4" :key="o" class="text item">
          {{'列表内容 ' + o }}
        </div>
      </el-card>
    </el-header>
    <el-container>
      <el-aside width="200px">
        <el-menu 
          default-active="1"
          class="el-menu-vertical-demo">
          <el-menu-item index="1">
            <i class="el-icon-setting"></i>
            <span slot="title">本年度</span>
          </el-menu-item>
          <el-menu-item index="2">
            <i class="el-icon-setting"></i>
            <span slot="title">半年</span>
          </el-menu-item>
          <el-menu-item index="3">
            <i class="el-icon-setting"></i>
            <span slot="title">三个月</span>
          </el-menu-item>
          <el-menu-item index="4">
            <i class="el-icon-setting"></i>
            <span slot="title">本月</span>
          </el-menu-item>
          <el-menu-item index="5">
            <i class="el-icon-setting"></i>
            <span slot="title">本周</span>
          </el-menu-item>
          <el-menu-item index="6">
            <i class="el-icon-setting"></i>
            <span slot="title">本日</span>
          </el-menu-item>
        </el-menu>
      </el-aside>
      <el-main>
        <el-row>
          <el-col :span="16">
            <div class="grid-content bg-purple">
              <el-row>
                <el-col :span="24">
                  <div class="grid-content bg-purple-dark">
                    流入流出统计
                  </div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="12">
                  <div class="grid-content bg-purple">
                    来源地总数TOP10
                  </div>
                </el-col>
                <el-col :span="12">
                  <div class="grid-content bg-purple-light">
                    流入人口年龄段统计
                  </div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="12">
                  <div class="grid-content bg-purple">
                    流出地总数TOP10
                  </div>
                </el-col>
                <el-col :span="12">
                  <div class="grid-content bg-purple-light">
                    流出人口年龄段统计
                  </div>
                </el-col>
              </el-row>
            </div>
          </el-col>
          <el-col :span="8">
            <div class="grid-content bg-purple-light">
              流入重点人员信息
            </div>
            <person-msg-s></person-msg-s>
            <person-msg-s></person-msg-s>
            <person-msg-s></person-msg-s>
            <div class="grid-content bg-purple-light">
              流出重点人员信息
            </div>
            <person-msg-s></person-msg-s>
            <person-msg-s></person-msg-s>
            <person-msg-s></person-msg-s>
          </el-col>
        </el-row>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
  import personMsgS from 'components/person-msg-s/person-msg-s'

  export default {
    name: 'Home',
    data () {
      return {
      }
    },
    methods: {
    },
    components: {
      personMsgS
    }
  }
</script>

<style lang="less" scoped>
  .home{
    .el-container{
      padding: 20px 0 0 20px;
    }
    .el-main{
      overflow: initial;
      padding: 0 20px;
    }
    .el-row{
      .el-col{
        height: 50px;
      }
    }
  }
</style>
