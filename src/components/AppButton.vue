<template>
  <div class="button">
    <span>I'm a button!</span>
    <!-- eslint-disable -->
    <button
      type="button"
      @click="click"
    >
      <slot />
    </button>
    <!-- eslint-enable -->
  </div>
</template>

<script>
export default {
    name: 'AppButton',
}
</script>
