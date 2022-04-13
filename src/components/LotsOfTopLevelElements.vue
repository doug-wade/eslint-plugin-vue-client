<i18n locale="en">
Wow what is even happening this example is wild
</i18n>

<i18n locale="ja">
Go home Vue SFCs you're drunk
</i18n>

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

<style scoped>
div {
    background-color: blue;
}
</style>

<style>
h1 {
    color: red;
}
</style>

<docs>
This is documentation?
</docs>
