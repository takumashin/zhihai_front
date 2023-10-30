<template>
  <Swiper>
    <SwiperSlide></SwiperSlide>
  </Swiper>
</template>
<style scoped></style>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  setup() {
    return {
      newsData: [{
        img: '',
        title: '',
        content: '',
      }]
    }
  },
})
</script>
