<template>
  <div>
    <slot
      my-prop="foo"
      my-other-prop="bar"
    />
  </div>
</template>

<script>
export default {
    name: 'SlotProps'
}
</script>