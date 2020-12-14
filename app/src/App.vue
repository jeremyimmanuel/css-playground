<template>
  <div class="main-container">
    <!-- <card-one
      title="Grizz"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.v8-QAbCvzLeW61kDqjDmMAHaFZ%26pid%3DApi&f=1"
    />

    <card-one
      title="Panda"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.vYmmng-wR4t5upJhILvfmAAAAA%26pid%3DApi&f=1"
    />

    -->
    <card-one
      title="Ice Bear"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.ytimg.com%2Fvi%2F4X_aIGXtKJY%2Fmaxresdefault.jpg&f=1&nofb=1"
    />
    <card-two
      title="Doraemon"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.ytimg.com%2Fvi%2F0I9WPVx2rHU%2Fmaxresdefault.jpg&f=1&nofb=1"
    />
    <card-three />
    <card-four />

    <card-five />
  </div>
</template>

<script>
import CardOne from './components/CardOne';
import CardTwo from './components/CardTwo';
import CardThree from './components/CardThree';
import CardFour from './components/CardFour';
import CardFive from './components/CardFive';

export default {
  name: 'App',
  components: {
    CardOne,
    CardTwo,
    CardThree,
    CardFour,
    CardFive
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #cbeafb;
}

main-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  padding: 30px;
  width: 1100px;
}

</style>
