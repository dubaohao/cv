<template>
  <div id="app">
    <div class="header">
      <div class="header_logo">
        <h1>芝麻点小小仙</h1>
      </div>
      <nav>
        <div>
          <router-link to="/">Home</router-link>
        </div>
        <div>
          <router-link to="/project">Project</router-link>
        </div>
        <div>
          <router-link to="/blob">Blob</router-link>
        </div>
        <div>
          <router-link to="/todo">Todo</router-link>
        </div>
        <div>
          <router-link to="/resume">Resume</router-link>
        </div>
        <div><a href="https://github.com/dubaohao">github</a></div>
      </nav>
    </div>
    <div class="content">
      <router-view />
    </div>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <!-- <router-view /> -->
  </div>
</template>

<style scoped lang="scss">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    overflow: hidden;
  }

  .header {
    position: fixed;
    width: 100%;
    background: yellow;
    box-shadow: 1px 1px 1px;
    height: 50px;
    line-height: 50px;
    z-index: 100;

    & .header_logo {
      float: left;
      width: 20%;
      height: 50px;
      border: 1px #AA22FF solid;
      box-shadow: 3px 3px 5px #AA22FF;
    }
    @media screen and (max-width: 800px) {
    & .header_logo {
      float: left;
      width: 20%;
      height: 50px;
      border: 1px #AA22FF solid;
      box-shadow: 3px 3px 5px #AA22FF;
      font-size: 6px;
    }
}

    & nav {
      float: right;
      color: #000;
      overflow: hidden;
      & div {
        display: inline-block;
        width: 75px;
        font-family: "微软雅黑";
        font-size: 18px;
        margin: 0 auto;
      }
    }
  }

  .content {
//     position: absolute;
//     width: 100%;
//     margin-top: 50px;
//     margin-bottom: -200px;
//     height: 100%;
//     overflow-x: hidden;
  }

//     #nav {
//       padding: 30px;
//
//       a {
//         font-weight: bold;
//         color: #2c3e50;
//
//         &.router-link-exact-active {
//           color: #42b983;
//         }
//     }
//     }

</style>
