<template lang="pug">
div.Initial-test
  h1(:style="color") {{ heading }}
  button(@click="makeTextGreen") Make Text Green
</template>

<script lang="coffee">
export default
    name: 'InitialTest'
    data: () ->
        heading: 'Initial Test'
        color: 'color:blue'
    methods:
        makeTextGreen: ->
            @color = 'color:green'
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
h1
  font-style italic
</style>
