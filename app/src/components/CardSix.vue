<template>
  <div class="box" :class="{ 'box-clicked': isClicked }" @click="onClick"></div>
</template>

<script>
export default {
  name: "CardSix",

  data() {
    return {
      isClicked: false,
    };
  },

  methods: {
    onClick() {
      if (!this.isClicked) {
        this.isClicked = true;
        setTimeout(() => {
          this.isClicked = false;
        }, 4000);
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.box {
  background: white;
  height: 200px;
  width: 200px;
  position: relative;
  border-radius: 8px;
  transition: all;
  transition-duration: 1s;
}
.box:active {
  // animation-name: myanimation;
  // animation-duration: 4s;
  // animation-iteration-count: 1;
  transform: skewX(25deg);
}

@keyframes myanimation {
  0% {
    background-color: white;
    left: 0;
    top: 0;
  }
  25% {
    background-color: red;
    left: 300px;
    top: 0px;
  }
  50% {
    background-color: green;
    left: 300px;
    top: 300px;
  }
  75% {
    background-color: blue;
    left: 0;
    top: 300px;
  }
  100% {
    background-color: white;
    left: 0;
    top: 0;
  }
}
</style>