<template>
  <button @click="printMessage">Print message</button>
</template>

<script>

export default {
  name: 'App',
  props: {
    message: String,
    printMessage: {
      type: Function,
      default() {
        console.log(this.message);
      }
    }
  }
}
</script>
