<template>
  <div id="app">
    <div class="header">
      <img class="map" src="./assets/img/map.png" alt="">
      <img class="logo" src="./assets/img/logo.png" alt="">
      <div class="foot">
        <div class="des">数据来源：国家及各地卫健委每日信息发布 </div>
        <div class="help"></div>
      </div>
    </div>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <!-- <router-view/> -->
  </div>
</template>

<style lang="less">
@media screen and (min-width: 750px) {
  html {
    font-size: 75PX !important;
  }
}
html {
  height: 100%;
  background:linear-gradient(#00A2A2,#00CECE);
}
body {
  margin: 0 auto;
  min-width: 320PX;
  max-width: 750PX;
  width: 10rem;
  line-height: 1.5;
}


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  position: relative;

  .header {
    width: 100%;
    
    .map {
      width: 100%;
    }
    .logo {
      position: absolute;
      left: 40px;
      top: 80px;
      height: 225px;
    }
    .foot {
      top: 325px;
      left: 42px;
      position: absolute;
      height: 20px;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      align-content: center;
    }
    .des {
      font-size: 12px;
      color: #fff;
    }
    .help {
      margin-left: 6px;
      width: 20px;
      height: 20px;
      background: url('./assets/img/help.png') no-repeat;
      background-size: 100%;
    }
  }
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
