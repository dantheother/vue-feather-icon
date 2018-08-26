<template>
  <component :is="name"></component>
</template>
<script>
  export default {
    props: ['type'],
    computed: {
      name() {
        return `feather-${this.type}`
      }
    }
  }
</script>
