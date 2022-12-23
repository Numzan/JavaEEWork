<template>
  <div>
    <el-card>
      <div id="line" style="width: 100%; height: 400px">欢迎！！</div>
    </el-card>
  </div>
</template>

<script>
import Cookies from 'js-cookie'
import request from "@/utils/request";
import * as echarts from 'echarts'


  export default {
    data() {
      return {
        admin: Cookies.get('admin') ? JSON.parse(Cookies.get('admin')) : {},
      }
    },
    mounted() {
      this.load()
    },
    methods: {

    }
  }
</script>

<style>
.input {
  width: 300px;
}
</style>
