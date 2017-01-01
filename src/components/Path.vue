<template lang="pug">
  div#path
    svg
      path(d="M10 10 h 80 v 80 h -80 Z" fill="transparent" stroke="black")
      circle(cx="10" cy="10" r="2" fill="red")
      circle(cx="90" cy="90" r="2" fill="red")
      circle(cx="90" cy="10" r="2" fill="red")
      circle(cx="10" cy="90" r="2" fill="red")
      path(d="M100 100 h 80 v 80 h -80 Z" stroke="black" class="next-path")
      <!--贝塞尔曲线，大写是绝对定位，小写是相对-->
      path(d="M200 10 c 70 20, 120 20, 160 0" stroke="black" fill="transparent")
    svg#svg_bessel
      path(d="M10 80 C 40 10, 65 10, 95 80 S 150 150, 180 80" stroke="black" fill="transparent")
      path(d="M100 100 Q 200 150, 100 250" fill="#f1f1f8")
    svg#svg_arc
      path(d="M10 315 L 110 215 A 30 50 0 0 1 162.55 162.45 L 172.55 152.45 A 30 50 -45 0 1 215.1 109.9 L 315 10" stroke="black" fill="green" stroke-width="2" fill-opacity="0.5")
</template>
<script>
export default {
  name: 'pathDemo',
  data () {
    return {}
  }
}
</script>

<style scoped>
  svg { border:1px dashed #c1c1c1; width:80%; height:300px; }
  .next-path {fill: #c3c3c3;}
</style>
