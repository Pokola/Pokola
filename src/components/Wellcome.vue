<template>
  <div class="hello">
    <h1 class="h1">{{msg}}</h1>
    <div class="anim-test">hello~!</div>
  </div>
</template>

<script>
export default {
  name: 'Wellcome',
  data () {
    return {
      msg: 'Welcome'
    }
  }
}
</script>

<style scoped lang="scss">
$font : 24px !default;
$color: #6DCCD0 !default;
.h1 {
  font-size: $font;
  color: $color;
}
.anim-test {
  box-sizing: border-box;
  width: 100px;
  height: 100px;
  margin-left: 100px;
  background: #D6D6D6;
  color: #fff;
  text-align: center;
  line-height: 100px;
  transform: rotate(30deg);
  transition: transform .4s;
  &:hover {
    transform: rotate(-30deg);
  }
}
</style>
