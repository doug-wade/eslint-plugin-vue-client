<template>
  <div class="non-compliant-button">
    <span>I'm non-compliant!</span>
    <button
      type="button"
      @click="click"
    >
      <slot />
    </button>
  </div>
</template>

<script>
export default {
    name: 'NonCompliantButton',
}
</script>