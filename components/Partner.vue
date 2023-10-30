<template>
  <div class="partner">
    <h5 class="partner-title">合作伙伴</h5>
    <p class="parter-subtitle">我们的客户以及我们的供应商</p>
    <div class="partner-content">
      <div class="partner-card">
        <img src="~assets/image/cw.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/lg.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/jabil-l.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/nokia-l.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/flex.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/hp.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/yamada.png" />
      </div>
      <div class="partner-card">
        <img src="~assets/image/foxconn-l.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    partner: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.partner {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 1rem;
}

.partner-title {
  font-size: 28px;

}

.partner img {
  max-width: 100%;
  height: auto;
  margin-bottom: 1rem;
}

.partner h5 {
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.partner p {
  font-size: 1.2rem;
  margin: 0.5rem 0 1rem 0;
}

.partner-content {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.partner a {
  font-size: 1rem;
  color: #0070f3;
  text-decoration: none;
}

.partner-card img {
  display: block;
  border: 1px solid #fff;
  margin: 0;
  width: 100%;
  height: 100%;
}
.partner-card {
  width: 160px;
  margin: 0 20px;
}
</style>
