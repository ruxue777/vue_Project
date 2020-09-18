<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HW msg="测试git！"/>
    <div class="select_box">
      <div class="select_item" @click="selected=!selected" v-if="selected == false">A</div>
      <div class="select_item" @click="selected=!selected" v-else>B</div>
    </div>
  </div>
</template>

<script>
import HW from './components/HelloWorld.vue'

export default {
  components: {
    HW 
  },
  data(){
    return {
      selected:true
    }
  },
  watch:{
    selected:function(e){
      console.log(e);
    }
  }
}
</script>

<style lang="less" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.select_box{
  width: 100% - 1px;
  height: 500px;
  display: flex;
  justify-content: center;
  align-content: center;
  border: 1px solid #000000;
  padding: 10px;

  .select_item{
    width: 100%;
    height: 100%;
    background: pink;
    display: flex;
    align-content: center;
    justify-content: center;
    font-size: 30px;
  }
} 
</style>
