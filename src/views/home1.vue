<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class ="left">
      <h1>姓名：杜保皓</h1>
      <h1>学校：北京邮电大学</h1>
      <h1>学历：硕士研究生</h1>
    </div>
    <div class ="right">
      <h1>姓名：<input value="杜保皓"/></h1>
      <h1>学校：<input value="北京邮电大学"/></h1>
      <h1>学历：<input value="硕士研究生"/></h1>
    </div>
  </div>

</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
<style lang="scss">
  .home{
    width:100%;
    height: 100%;
    position:absolute;
    /* vertical-align: middle; */
  }
  .left{
    float:left;
    width:40%;
    margin-top:100px;
    margin-left:50px;
    border:red 1px dashed;
    box-shadow: 1px 1px 1px #E9E9E9;
    height:60%;
    & h1{
      position: relative;
    margin:5px 0 0 10px;
      }
  }
  .right{
    float:right;
    width:40%;
    margin-top:100px;
    margin-right:50px;
    border:blue 1px dotted;
    box-shadow: 1px 1px 1px #E9E9E9;
    height:60%;
    & h1{
      position: relative;
      margin:5px 0 0 10px;
    }
  }
</style>
