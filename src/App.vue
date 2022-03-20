<template>
  <img
    alt="Vue logo"
    src="./assets/logo.png"
  >
  <Button @click="buttonClickHandler">
    Compliant
  </Button>
  <NonCompliantButton @click="nonCompliantButtonHandler">
    Non Compliant
  </NonCompliantButton>
  <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Button from './components/Button.vue'
import NonCompliantButton from './components/NonCompliantButton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Button,
    NonCompliantButton,
  },
  methods: {
    buttonClickHandler() {
      console.log('clicked compliant button');
    },
    nonCompliantButtonHandler() {
      console.log('clicked non-compliant button');
    }
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
</style>
