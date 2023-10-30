<template>
  <div class="banner">

    <div class="banner-content">
      <h1>{{ title }}</h1>
      <p>{{ subtitle }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: false,
      default: 'Default Title'
    },
    subtitle: {
      type: String,
      required: false,
      default: '以人为本 精益求精 打造行业内一流企业'
    },
    videoSrc: {
      type: String,
      required: false,
      default: 'https://image-1251389146.file.myqcloud.com/videobanner.mp4'
    }
  }
}
</script>

<style lang="scss" scoped>
.banner {
  position: relative;
  height: 100vh;
  overflow: hidden;
  padding-top: 50px;
  width: 100%;
  &::after {
    content: '';
    display: block;
    top: 0;
    position: absolute;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.6);
  }
}

video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.banner-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #fff;
  z-index: 3;

  width: 100%;
  max-width: 1140px;
  max-height: 840px;
  padding: 8rem 6rem;
  background: rgba(255, 255, 255, 0.375);
  box-shadow: 0 0.75rem 2rem 0 rgba(0, 0, 0, 0.1);
  border-radius: 2rem;
  border: 1px solid rgba(255, 255, 255, 0.125);
}

h1 {
  font-size: 4rem;
  margin-bottom: 2rem;
}

p {
  font-size: 2rem;
  margin-bottom: 2rem;
}

button {
  font-size: 2rem;
  padding: 1rem 2rem;
  background-color: #fff;
  color: #000;
  border: none;
  border-radius: 2rem;
  cursor: pointer;
}
</style>
