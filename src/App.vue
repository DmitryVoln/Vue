<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" style="width: 100px; height: 100px; margin: auto">
    
    Welcome to: {{calculator}}
    <Calc/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Calc from './components/Calc.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Calc,
  },
  data: () => ({
    calculator: 'calculator'
  })
}
</script>

<style lang="scss">
#app {
  display: flex;
  flex-direction: column;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.btn {
  width: 50px;
  margin:  auto;
}
.calc {
  display: flex;
  justify-content: space-around;
}
.result {
  border: solid 1px #000;
  width: 100px;
}
</style>
