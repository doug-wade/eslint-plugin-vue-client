<template>
  <some-random-name />
</template>

<script>
import NonCompliantButton from './NonCompliantButton.vue'

const someRandomName = '' + Math.random();

export default {
  name: 'ImportComponentName',
  components: {
    [someRandomName]: NonCompliantButton,
  }
}
</script>
