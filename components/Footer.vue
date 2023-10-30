<template>
  <footer>
    <div class="footer-container">
      <div class="footer-nav">
        <ul>
          <li>产品介绍</li>
          <li>解决方案</li>
          <li>关于我们</li>
          <li>新闻中心</li>
        </ul>
        <div>
          <div class="footer-sales-btn">联系销售</div>
        </div>
      </div>
      <div class="footer-content">
        <div class="footer-logo">
        </div>
        <p class="footer-address-text">地址：深圳市光明新区白花社区第一工业区志海工业园</p>
        <p class="footer-address-text">联系电话：0755-29970300</p>
        <div class="footer-social">
          <div class="footer-qq"></div>
          <div class="footer-wechat"></div>
        </div>
      </div>
      <div class="copyright">Copyrights@{{ year }} 志海精密配件(深圳)有限公司 粤ICP备05044766号</div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      year: 2023
    }
  },
  mounted() {
    let date = new Date()
    this.year = date.getFullYear()
  }
}
</script>

<style lang="scss" scoped>
.footer-nav ul {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  background: #0055BE;
}
.footer-nav ul li{
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  padding: 0 20px;
  height: 50px;
  line-height: 50px;
  background: #0055BE;
}

.footer-content {
  margin: 0;
  padding: 0 30px;
  overflow: hidden;
}
.footer-sales-btn {
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  padding: 0 20px;
  height: 35px;
  line-height: 35px;
  border: 2px solid #fff;
  display: inline-block;
  border-radius: 25px;
  transition: all 0.3s ease-in-out;
  &:hover {
    background: #fff;
    color: #0055BE;
  }
}

.footer-logo {
  background: url('assets/image/index-logo.png') center center no-repeat;
  background-size: contain;
  width: 318px;
  height: 61px;
  font-size: 0;
  margin: 20px 0 20px 0;
}

.footer-nav {
  background: #0055BE;
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  padding: 10px 20px;
}

.footer-nav ul li {
  color: #fff;
  font-size: 16px;
  font-weight: 600;
  padding: 0 20px;
  margin: 0 10px;
  height: 50px;
  line-height: 50px;
}

.footer-nav ul li:hover {
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.5);
  transition: all 0.3s ease-in-out;
}

footer {
  background-color: #fff;
  padding: 0;
}

.copyright {
  color: #fff;
  background: #0055BE;
  padding: 15px 25px;
}

.container {
  max-width: 960px;
  margin: 0 auto;
}


h4 {
  font-size: 18px;
  margin-bottom: 20px;
}

p {
  font-size: 14px;
  line-height: 1.5;
  margin-bottom: 20px;
}

.social-icons {
  list-style: none;
  margin: 0;
  padding: 0;
}

.social-icons li {
  display: inline-block;
  margin-right: 10px;
}

.social-icons li:last-child {
  margin-right: 0;
}

.social-icons a {
  display: block;
  width: 30px;
  height: 30px;
  line-height: 30px;
  text-align: center;
  color: #fff;
  background-color: #333;
  border-radius: 50%;
  transition: all 0.3s ease-in-out;
}

.social-icons a:hover {
  transform: translateY(-5px);
}

.footer-address-text {
  text-align: left;
  font-size: 16px;
  margin: 0 0 10px 0;;
}
</style>
