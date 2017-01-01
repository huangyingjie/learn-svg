<template lang="pug">
  div#shape
    svg(width="80%" height="250" version="1.1" xmlns="http://www.w3.org/2000/svg")
      ellipse(cx="75" cy="75" rx="50" ry="20" stroke="red" fill="transparent" stroke-width="5")
      line(x1="10" x2="200" y1="120" y2="140" fill="#f1f1f1" stroke="#c3c3c3" stroke-width='3')
      polyline(stroke="orange" points="200 30, 210 40, 220 50, 210 60, 200 70" stroke-width="2" fill="transparent")
      polygon(stroke="#e2e2e2" stroke-width="4" fill="transparent" points="50 160, 55 180, 70 180, 60 190, 65 205, 50 195, 35 205, 40 190, 30 180, 45 180")
      <path d="M20,230 Q40,205 50,230 T90,230" fill="none" stroke="blue" stroke-width="5"/>
</template>
<script>
export default {
  name: 'shape',
  data () {
    return {}
  }
}
</script>
<style scoped>
  svg { border:1px dashed #c1c1c1; }
  ellipse { transition:all 2s; }
  ellipse:hover { stroke:green; stroke-width:10; }
</style>
