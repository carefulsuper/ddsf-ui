<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Demo/>
    <m-card imgSrc="java.jpg" summary="Java是最牛逼的后台语言" />
    <br/>
    <m-card imgSrc="vue.jpg" summary="Vue.js是最牛逼的前端框架">
      <template v-slot:footer>
        <div class="footer">
          <div class="level">中级·528人报名</div>
          <div class="price">￥299.00</div>
        </div>
      </template>
    </m-card>
    <br/>
    <m-card imgSrc="spring.jpg" :width="370" :imgHeight="190">
      <template>
        本路线旨在帮助想快速掌握Springboot应用的工程师，全方位多角度带你升级。
      </template>
      <template v-slot:footer>
        <div class="footer-spring">
          <div class="level">4步骤·6门课</div>
          <div class="price">￥299.00</div>
        </div>
      </template>
    </m-card>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.footer {
  padding: 0;
  font-size: 12px;
  text-align: left;
}

.level {
  color: #9199A1;
  margin-bottom: 8px;
}

.price {
  color: #F01414;
}

.footer-spring {
  display: flex;
  justify-content: space-between;
  padding: 0 8px;
  font-size: 12px;
}
</style>
