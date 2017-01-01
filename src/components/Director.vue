<template lang="pug">
  ul.nav.fixed
    li
      a(href="#coordinate") 坐标系
    li
      a(href="#shape") 基本形状
    li
      a(href="#path") 路径(path)
      ul
        li
          a(href="#svg_bessel") 贝塞尔曲线
        li
          a(href="#svg_arc") 弧形
    li
      a(href="#stroke") 边框(Stroke)
      ul
        li
          a(href="#svg_linecap") linecap
        li
          a(href="#svg_linejoin") linejoin
        li
          a(href="#svg_dasharray") dasharray
    li
      a(href="#gradient") Gradient渐变
      ul
        li
          a(href="#svg_linearGradient") 线性渐变
        li
          a(href="#svg_radialGradient") 径向渐变
</template>
<script>
export default {
  name: 'director',
  components: {
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
<style scoped>
.fixed { position:fixed; top:0; }
</style>
