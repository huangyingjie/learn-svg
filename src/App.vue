<template lang="pug">
  div.container
    div#app.row
      div.col-md-3
        director
      div.col-md-9
        coordinate
        shape
        pathDemo
</template>

<script>
import Director from './components/Director'
import Coordinate from './components/Coordinate'
import Shape from './components/Shape'
import PathDemo from './components/Path'

export default {
  name: 'app',
  components: {
    Coordinate,
    PathDemo,
    Shape,
    Director
  }
}
</script>

<style scoped>
</style>
