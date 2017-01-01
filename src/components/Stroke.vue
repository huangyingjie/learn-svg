<template lang="pug">
  div#stroke
    svg#svg_linecap
      <line x1="40" x2="120" y1="20" y2="20" stroke="black" stroke-width="20" stroke-linecap="butt"/>
      <line x1="40" x2="120" y1="60" y2="60" stroke="black" stroke-width="20" stroke-linecap="square"/>
      <line x1="40" x2="120" y1="100" y2="100" stroke="black" stroke-width="20" stroke-linecap="round"/>
    svg#svg_linejoin
      polyline(points="40 60 80 20 120 60" stroke="black" stroke-width="20" stroke-linecap="butt" fill="none" stroke-linejoin="miter")
      polyline(points="140 60 180 20 220 60" stroke="black" stroke-width="20" stroke-linecap="round" fill="none" stroke-linejoin="round")
      polyline(points="260 60 300 20 340 60" stroke="black" stroke-width="20" stroke-linecap="square" fill="#c9c9c9" stroke-linejoin="bevel")
    svg#svg_dasharray
      path(d="M 10 75 Q 50 10 100 75 T 190 75" stroke="black" stroke-linecap="round" stroke-dasharray="5,10,5" fill="none")
      path(d="M 10 75 L 190 75" stroke="red" stroke-linecap="round" stroke-width="1" stroke-dasharray="5,5" fill="none")
</template>
<script>
export default {
  name: 'stroke',
  data () {
    return {}
  }
}
</script>

<style scoped>
  svg { border:1px dashed #c1c1c1; width:80%;}
  #svg_linecap line { stroke:purple; transition:all 2s; }
  #svg_linecap line:hover { stroke:green;cursor:pointer; }
</style>
