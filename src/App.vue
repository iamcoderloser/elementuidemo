<template>
  <div id="app">
    <HelloWorld>
      <span slot='slotc'>槽口C</span>
			<span slot='slotb'>槽口B</span>
			槽口A
    </HelloWorld>
    <div>{{loading}}xxx</div>

    <el-button type="primary" :loading="loading">加载中</el-button>
  </div>


</template>



<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      loading:true
    }
  },
  mounted() {
    var that = this;
    setTimeout(() => {
      that.loading = false;
    }, 5000);
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


</style>
