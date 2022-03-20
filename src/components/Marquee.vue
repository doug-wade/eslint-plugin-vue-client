<template>
  <marquee>{{ msg }}</marquee>
</template>

<script>
export default {
    name: "Marquee",
    propsData: {
        msg: {
            type: String,
            default: ""
        }
    }
}
</script>