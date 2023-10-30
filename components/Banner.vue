<template>
  <div class="banner">
    <video autoplay loop muted>
      <source :src="videoSrc" type="video/mp4">
    </video>
    <div class="banner-content">
      <h1><span>{{ title }}</span></h1>
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
      default: '志海精密配件有限公司'
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
  
}

h1 {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  font-size: 4rem;
  margin-bottom: 2rem;
  font-weight: 200;
  font-family: 'nst';
  white-space: nowrap;
  &::before {
    content: '';
    position: relative;
    width: 120px;
    height: 120px;
    display: block;
    background: url('assets/image/kt-logo.jpg') center center no-repeat;
    background-size: contain;
    margin: 0 20px 0 0;
  }
  span {
    display: block;
  }
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
