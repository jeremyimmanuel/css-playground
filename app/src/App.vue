<template>
  <div class="main-container">
    <card-one
      title="Grizz"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.v8-QAbCvzLeW61kDqjDmMAHaFZ%26pid%3DApi&f=1"
    />

    <card-one
      title="Panda"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.vYmmng-wR4t5upJhILvfmAAAAA%26pid%3DApi&f=1"
    ></card-one>

    <card-one
      title="Ice Bear"
      imgLink="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.ytimg.com%2Fvi%2F4X_aIGXtKJY%2Fmaxresdefault.jpg&f=1&nofb=1"
    />
  </div>
</template>

<script>
import CardOne from './components/CardOne';

export default {
  name: 'App',
  components: {
    CardOne
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
  background: #490f25;
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
