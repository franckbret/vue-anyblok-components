<template>
  <div class="component-b">
    <slot><h1>{{ value }}</h1></slot>
    <input type="text" v-model="value">
    <button @click="myBaseEvent">Click me</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      value: 'Vue'
    }
  },
  methods: {
    myBaseEvent () {
      this.$emit('click', this.value)
      console.log('Message emit from base component')
    }
  }
}
</script>

<style lang="scss" scoped>
.component-b {
  color: #ff0000;
}
</style>
