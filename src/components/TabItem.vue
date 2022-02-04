<template>
  <button @click="$emit('input', id)" :class="[active, 'tab']">
    {{ label }}
  </button>
</template>

<script>
export default {
  props: {
    id: Number,
    label: String,
    value: Number
  },
  computed: {
    active() {
      return this.value === this.id ? 'active' : false
    }
  }
}
</script>

<style scoped>
.tab {
  background: purple;
  color: green;
  width: 30%;
  font-size: 200%;
}
.tab:hover {
  background: #eeeeee;
}
.active {
  background: #f7c9c9;
}
</style>