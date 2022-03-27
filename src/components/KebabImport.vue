<template>
  <div>
    <app-button />
    <epvc-app-marquee />
  </div>
</template>

<script>
import AppButton from './AppButton.vue'
import AppMarquee from './AppMarquee.vue'

export default {
    name: 'KebabImport',
    components: {
        'app-button': AppButton,
        'epvc-app-marquee': AppMarquee,
    }
}
</script>