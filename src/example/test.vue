<template>
<div class="container">
    <div class="menu">
      <el-tabs v-model="activeName" @tab-click="handleClick">
        <el-tab-pane label="首页" name="first">这是首页</el-tab-pane>
        <el-tab-pane label="帮助" name="second">有什么问题</el-tab-pane>
        <el-tab-pane label="关于" name="third">关于我们</el-tab-pane>
        <el-tab-pane label="更多" name="fourth">了解更多</el-tab-pane>
      </el-tabs>
    </div>
    <div id="form1">
        <ul>
         <li>姓名：<el-input v-model="form.name"></el-input></li>
          <el-radio class="radio" v-model="form.radio" label="1">男</el-radio>
          <el-radio class="radio" v-model="form.radio" label="2">女</el-radio>
        </ul>
      <button @click="getData">更换数据</button>
      <el-button type="primary" @click="getData">更换数据</el-button>
      <router-link to="/memu1">导航一</router-link>
      <router-link to="/memu2">导航二</router-link>
      <router-view></router-view>
    </div>
</div>
</template>
<script>
  export default {
    data () {
      return {
        activeName: 'second',
        form: {
          name: '张三',
          radio: '1'
        }
      }
    },
    methods: {
      handleClick (tab, event) {
        console.log(tab, event)
      },
      getData () {
        this.$http.get('../../static/resourceData.json', {params: {'key': this.inputValue}}).then(function (response) {
          console.log(response)
          console.log('这是我们需要的json数据', response.data)
          this.form = response.data
        }, function (response) {
          alert('请求失败了')
        })
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body{
  padding:0;
  margin:0 auto;
}
.container{
	width:500px;
  margin:auto;
}
#form1{
  margin-top:100px;
  border: 1px solid red;
}
.el-input, .el-input__inner {
    width: 30%;
    display: inline-block;
}
li{
  list-style:none;
}
</style>
