<template>
  <div v-for="cont in conts" :key="cont.id"><input type="checkbox" value="1">{{cont.text}}</div>
</template>

<script>
export default {
  name: "ToItem",
  data(){
    return {
      conts: [
        {id: 1, text: "one"}
      ]
    }
  },
}
</script>

<style>

</style>