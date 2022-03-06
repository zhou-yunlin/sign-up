<template>
  <!--<img alt="Vue logo" src="./assets/logo.png">alt:如果无法显示图像，浏览器将显示替代文本-->
  <div id="backgruand">
    <img alt="Vue logo" src="./assets/水彩.jpg">
  </div>
  <HelloWorld msg="Login"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
.background{
  background: url(./assets/图3.jpg) no-repeat;/*图片不重复*/
  background-size: cover;/*把背景图扩展至足够大，直至完全覆盖背景区域，图片比例保持不变且不会失真，但某些部分被切割无法显示完整背景图像*/
  background-attachment: fixed;/*图片不随浏览器滚动*/
}
</style>
