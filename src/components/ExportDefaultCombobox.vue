<template>
  <div>
    <input type="text">
    <select />
    <AppButton />
    <SlotProps />
  </div>
</template>

<script>
import AppButton from './AppButton.vue'
import SlotProps from './SlotProps.vue'

export default {
     name: 'ExportDefaultCombobox',
     components: {
         AppButton,
         SlotProps,
     }
}
</script>