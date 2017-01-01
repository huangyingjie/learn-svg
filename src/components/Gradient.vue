<template lang="pug">
  div#gradient
    svg#svg_linearGradient
      defs
        linearGradient#Gradient1
          <stop class="stop1" offset="0%"/>
          <stop class="stop2" offset="50%"/>
          <stop class="stop3" offset="100%"/>
        linearGradient(id="Gradient2" x1="0" x2="0" y1="0" y2="1")
          <stop offset="0%" stop-color="red"/>
          <stop offset="50%" stop-color="black" stop-opacity="0"/>
          <stop offset="100%" stop-color="blue"/>
      rect(id="rect1" x="10" y="10" rx="15" ry="15" width="100" height="100")
      rect(x="210" y="10" rx="15" ry="15" width="100" height="100" fill="url(#Gradient2)")
    svg#svg_radialGradient
      defs
        radialGradient#RadialGradient1
          stop(offset="0%" stop-color="red")
          stop(offset="100%" stop-color="blue")
        radialGradient(id="RadialGradient2" cx="0.5" cy="0.5" r="0.25")
          stop(offset="0%" stop-color="red")
          stop(offset="100%" stop-color="blue")
      rect(x="10" y="10" rx="15" ry="15" width="100" height="100" fill="url(#RadialGradient1)")
      rect(x="210" y="10" rx="15" ry="15" width="100" height="100" fill="url(#RadialGradient2)")
</template>

<script>
export default {
  name: 'gradient'
}
</script>

<style scoped>
  svg { border:1px dashed #c1c1c1; width:80%;}
  #rect1 { fill: url(#Gradient1); }
  .stop1 { stop-color: red; }
  .stop2 { stop-color: black; stop-opacity: 0.5; }
  .stop3 { stop-color: blue; }
</style>
