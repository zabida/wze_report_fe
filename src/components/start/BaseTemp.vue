<template>
  <button @click="count++">click nu {{count}}</button>
  <div>{{ti}}</div>
  <div>
    <strong>This is an Error</strong>
    <slot/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  props: {
    ti: String
  }
}
</script>

<style scoped>

</style>