<template>
  <section class="clearAllContainer">
      <span class="clearAllBtn" v-on:click="clearTodo">Clear All</span>
  </section>
</template>

<script>
export default {
  methods: {
    clearTodo () {
      this.$emit('clearTodo')
    }
  }
}
</script>

<style scoped>
.clearAllContainer {
  width: 8.5em;
  height: 50px;
  line-height: 50px;
  background-color: #fff;
  border-radius: 5px;
  margin: 0 auto;
}
.clearAllBtn {
  color: #e20303;
  display: block;
}
</style>
