<template>
  <nav>
    <ul>
      <li class="logo"><nuxt-link to="/">Home</nuxt-link></li>
    </ul>
    <div>
      <ul class="subnav-group">
        <li class="subnav"><nuxt-link to="/product">产品介绍</nuxt-link></li>
        <li class="subnav"><nuxt-link to="/about">走进志海</nuxt-link></li>
        <li class="subnav"><nuxt-link>企业愿景</nuxt-link></li>
        <li class="subnav"><nuxt-link>研发与生产</nuxt-link></li>
        <li class="subnav"><nuxt-link>印刷业务</nuxt-link></li>
        <li class="subnav"><nuxt-link>新闻中心</nuxt-link></li>
        <li class="subnav"><nuxt-link>联系我们</nuxt-link></li>
      </ul>
      <div class="contact">
        <div class="contact-text">联系电话</div>
        <div class="contact-num">0755-29970300</div>
      </div>
    </div>
    
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style>
nav {
  background: linear-gradient(90deg, #FFF 15.21%, #0055BE 70.85%);
  box-shadow: 0px 3px 6px 0px rgba(0, 0, 0, 0.25);
  color: #fff;
  display: flex;
  justify-content: space-between;
  width: 100%;
  position: fixed;
  z-index: 2;
  height: 100px;
}

.logo {
  background: url('assets/image/index-logo.png') center center no-repeat;
  background-size: contain;
  width: 318px;
  height: 61px;
  font-size: 0;
  margin: 20px 45px;
}

ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
  height: auto;
}

a {
  color: #fff;
  text-decoration: none;
}
</style>
