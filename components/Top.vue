<template>
  <Swiper
    :height="300"
    :loop="true"
    :autoplay="{
      delay: 1000,
      disableOnInteraction: true
    }"
  
  >
    <SwiperSlide>
      <Banner title="志海精密配件有限公司" subtitle="全国领先的模具加工企业" />
    </SwiperSlide>
    <SwiperSlide>
      <SubBanner />
    </SwiperSlide>
    <SwiperSlide>
    </SwiperSlide>
  </Swiper>
</template>
<style scoped></style>