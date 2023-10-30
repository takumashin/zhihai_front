<template>
  <div>
    <!-- <NuxtWelcome /> -->
    <Navbar />
    <Top />
    <Goods />
    <NewsIndex />
    <Intro />
    <Partner />
    <Footer />
  </div>
</template>
<style scoped>
.swiper-slide {
  height: 100vh;
}
</style>
<script setup>
useHead({
  title: '志海精密配件(深圳)有限公司',
  meta: [
    { name: 'description', content: '志海精密配件(深圳)有限公司' },
    { name: 'keywords', content: '印刷品,志海精密配件(深圳)有限公司' },
    { name: 'author', content: '' },
    { name: 'viewport', content: 'width=device-width, initial-scale=1.0' },
  ],
  link: [
    { rel: 'icon', type: 'image/x-icon', href: 'assets/favicon/favicon.ico' },
  ],
})
</script>