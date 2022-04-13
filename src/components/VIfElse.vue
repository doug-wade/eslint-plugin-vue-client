<template>
  <div>
    <div v-if="conditional">
      foo
    </div>
    <div v-else>
      bar
    </div>
  </div>
</template>

<script>
export default {
    name: 'VIfElse',
    data() {
        return {
            conditional: false,
        };
    }
}
</script>