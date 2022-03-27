<template>
  <some-random-name />
</template>

<script>
import NonCompliantButton from './NonCompliantButton.vue'

export default {
    name: 'ImportComponentName',
    components: {
        'some-random-name': NonCompliantButton,
    }
}
</script>
