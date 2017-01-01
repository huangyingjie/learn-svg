<template lang="pug">
  div.container
    div#app.row
      div.col-md-3
        director
      div.col-md-9
        coordinate
        shape
        pathDemo
        stroke
        gradient
</template>

<script>
import Director from './components/Director'
import Coordinate from './components/Coordinate'
import Shape from './components/Shape'
import PathDemo from './components/Path'
import Stroke from './components/Stroke'
import Gradient from './components/Gradient'

export default {
  name: 'app',
  components: {
    Coordinate,
    Gradient,
    PathDemo,
    Shape,
    Stroke,
    Director
  }
}
</script>

<style scoped>
</style>
