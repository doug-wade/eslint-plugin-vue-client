<template>
  <img
    alt="Vue logo"
    src="./assets/logo.png"
  >
  <AppButton @click="buttonClickHandler">
    Compliant
  </AppButton>
  <NonCompliantButton @click="nonCompliantButtonHandler">
    Non Compliant
  </NonCompliantButton>
  <AppMarquee msg="Welcome to Your Vue.js App" />
  <SlotProps>
    <div>I'm a slot!</div>
  </SlotProps>
</template>

<script>
import AppMarquee from './components/AppMarquee.vue'
import AppButton from './components/AppButton.vue'
import NonCompliantButton from './components/NonCompliantButton.vue'
import SlotProps from './components/SlotProps.vue'

export default {
  name: 'App',
  components: {
    AppMarquee,
    AppButton,
    NonCompliantButton,
    SlotProps,
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
