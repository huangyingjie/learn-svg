<template lang="pug">
  div#coordinate
    svg(width="200" height="200" viewBox="0 0 100 100")
      rect(x="0" y="0" width="100" height="100" fill="#c9c9c9")
      text(x="50" y="50") 放大两倍
</template>
<script>
export default {
  name: 'coordinate',
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
  svg { border:1px dashed #c1c1c1; }
  text {font-size:12px;}
</style>
