<template>
  <div class="body_dbh_home">
    <div class="avatar_dbh_home">
      <div class="avatar1_dbh_home"></div>
      <!-- <Avatar shape="square" icon="ios-person" size="large" /> -->
    </div>
    <div class="content_dbh_home">
      <div class="ddd">
        <h1>姓名：</h1><span>杜保皓</span>
      </div>
      <div class="ddd">
        <h1>学校：</h1><span>北京邮电大学</span>
      </div>
      <div class="ddd">
        <h1>学历：</h1><span>硕士研究生</span>
      </div>
      <div class="ddd">
        <h1>职位：</h1><span>前端工程师</span>
      </div>
      <div class="ddd">
        <h1>目标：</h1><span>全栈工程师</span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'home',
  data () {
    return {}
  }
}

</script>
<style lang="scss">
  .body_dbh_home {
    position: absolute;
    width: 100%;
    height: 100%;
    background:url(../assets/27.jpg) center 50px no-repeat;
    background-size: 105% 100%;
    text-align: left;
  }

  .body_dbh_home:hover {}

  .avatar_dbh_home {
    // position:relative;
    float: left;
    width: 200px;
    height: 200px;
    margin: 300px 0 0 150px;
    border: 2px #000000 solid;
    border-radius: 50px;
    background: #FFF center center no-repeat;
    background-size: 150px 150px;
  }

  .avatar1_dbh_home {
    width: 150px;
    height: 150px;
    margin: 25px auto;
    border: 5px yellow solid;
    vertical-align: middle;
    border-radius: 100px;
    background:url(../assets/20190326104606.jpg) center center no-repeat;
    background-size: cover;
    // background-size: 120px 120px;
  }

  .avatar1_dbh_home:hover {
    background:url(../assets/dubaohao.jpg) center center no-repeat;
    background-size: contain;
    transition-duration: 2s;
    transform: rotateX(360deg);
    transition-timing-function: ease;
    transform-style: preserve-3d;
  }
  .content_dbh_home {
    float: right;
    // position: relative;
    width: 400px;
    height: 400px;
    margin: -300px 100px 0 65%;
    border: 2px #000000 solid;
    border-radius: 50px;
    background: #FFF center center no-repeat;
    background-size: 150px 150px;
    font-family: "微软雅黑";
  }

  .ddd {
    position: relative;
    // float: left;
    height: 50px;
    line-height: 50px;
    width: 100%;
    margin: 20px 0 0 20px;
    display: block;

    & h1 {
      float: left;
      margin: 0 0 0 0;
      width: 80px;
      // display: block;
    }

    & span {
      font-size: 20px;
    }

    & span:hover {
      // transition: ;
      transition-delay: 0.1s;
      border: 3px #FF9800 dashed;
      box-shadow: 1px 1px 1px cornflowerblue;
    }
  }
</style>
