<template>
  <div>
    <h1>Hello World!</h1>
    <Button @click="console.log('foo')">
      Click me!
    </Button>
  </div>
</template>

<script>
export default {
    name: 'ScriptSetup',
    mounted() {
        console.log('mounted')
    }
}
</script>

<script setup>
import Button from '../Button.vue'
</script>

<style>
h1 {
    color: red;
}
</style>
