<template>
  <marquee>{{ msg }}</marquee>
</template>

<script>
export default {
    name: "AppMarquee",
    propsData: {
        msg: {
            type: String,
            default: ""
        }
    }
}
</script>