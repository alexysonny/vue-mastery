<template lang='pug'>
.player
  slot
    .play-button
</template>


<script>
export default {
  name: 'player-placeholder'
}
</script>

<style lang='stylus' scoped>
@import '~assets/css/_variables'

.player
  height 200px
  width: 100%
  background-color $black
  display flex
  justify-self center
  align-items center
  justify-content center

  +tablet-up()
    height: 320px

  +laptop-up()
    height 440px

.play-button
  height 70px
  width 70px
  background-color #FFFFFF
  border-radius 50%
  display flex
  align-items center
  justify-content center

  &:after
    content ''
    width 0px
    height 0px
    border-top 12px solid transparent
    border-bottom 12px solid transparent
    border-left 20px solid $black
    margin-right -7px
</style>
