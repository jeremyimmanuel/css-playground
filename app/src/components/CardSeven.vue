<template>
  <div class="box"></div>
</template>

<script>
export default {
  name: "CardSeven",
};
</script>

<style lang="scss" scoped>
.box {
  background: white;
  width: 300px;
  height: 300px;
  position: relative;
  transition-property: all;
  transition-duration: 1s;
  transition-timing-function: ease-in-out;

  &:hover {
    background: red;
    border-radius: 50%;
    transform: rotateY(180deg) skewX(20deg) skew(0deg);
  }
}
</style>