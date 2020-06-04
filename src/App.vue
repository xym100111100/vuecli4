<template>
  <div id="app">
    <div class="header">
      <div class="leve">
        <img src="./assets/img/love.png" alt />
      </div>
      <div class="msg">
        <img src="./assets/img/msg.png" alt />
      </div>
    </div>
   <div class="main">
      <div class="main-content">
        <div class="content-title">最高可借(元)</div>
         <div class="content-money">10,000.00</div>
      <div class="content-btn">申请借款</div>
       <div class="content-remarks">
          <span>最低日费率0.05%</span>
          <span class="interval">|</span>
          <span>最快3分钟放款</span>
        </div>
         <div class="content-interval">
          <span v-for="i in 100" :key="i">-</span>
        </div>
         <div class="content-bill">账单金额(元)</div>
        <div class="content-bill-remarks">暂无借款</div>
      </div>
    </div>
    <div class="footer">
      <div class="footer-index">
        <div>
          <img src="./assets/img/index.png" alt />
        </div>
        <div>首页</div>
      </div>
      <div class="footer-my">
        <img src="./assets/img/my.png" alt />
        <div>我的</div>
      </div>
    </div>  
  </div>
</template>

<style>
body,
html {
  padding: 0;
  margin: 0;
}
#app {
  font-family: initial;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.header {
  display: flex;
  justify-content: space-between;
}
.header div {
  padding: 0.2rem;
  
}
.header img {
  height: 0.5rem;
}
.main {
  height: 100vh;
  background: url(./assets/img/back.png) no-repeat;
  background-size: 100%;
  display: flex;
  justify-content: center;
  background-color: #f5f5f5;
}
.main .main-content {
  height: 6.4rem;
  background: white;
  width: 6.4rem;
  margin-top: 21vh;
  border-radius: 0.15rem;
}

.main .main-content .content-title {
  text-align: center;
  margin-top: 0.5rem;
  font-size: 0.35rem;
  font-weight: bold;
}
.main .main-content .content-money {
  text-align: center;
  margin-top: 0.38rem;
  font-size: 0.6rem;
  font-weight: bold;
}

.main .main-content .content-btn {
  height: 1rem;
  text-align: center;
  line-height: 1rem;
  background: url(./assets/img/button.png) no-repeat;
  background-size: 100%;
  background-position:center;
  color: white;
  width: 63%;
  margin: 0.4rem auto 0;
  font-size: 0.4rem;
}
.content-remarks {
  width: 80%;
  margin: 0.3rem auto 0;
  text-align: center;
  color: #a8a4a4;
  font-size: 0.23rem;
  font-family: serif;
}
.content-remarks .interval {
  padding: 0 0.1rem;
}

.content-interval {
  width: 90%;
  margin: 0.1rem auto 0;
  color: #e6e1e1;
  font-weight: bold;
  font-size: 0.2rem;
  text-align: center;
  overflow: hidden;
  height: 0.2rem;
}
.content-bill {
  width: 90%;
  margin: 0.2rem auto 0;
  color: #a8a4a4;
  font-size: 0.23rem;
  font-family: serif;
}
.content-bill-remarks {
  width: 90%;
  margin: 0.2rem auto 0;
  font-weight: bold;
  font-size: 0.34rem;
}
.footer {
  background: white;
  height: 0.8rem;
  position: fixed;
  z-index: 100;
  bottom: 0;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  padding-top: 0.1rem;
}
.footer .footer-index {
  margin-left: 1rem;
  text-align: center;
  font-size: 0.2rem;
  color: red;
}
.footer .footer-my {
  margin-right: 1rem;
  text-align: center;
  font-size: 0.2rem;
  color: #cccccc;
}
.footer img {
  height: 0.4rem;
}
</style>
