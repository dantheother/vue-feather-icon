<template>
  <component :is="name" v-bind="componentProps"></component>
</template>
<script>
  export default {
    props: ['type', 'title'],
    computed: {
      name() {
        return `feather-${this.type}`
      },
      componentProps() {
        return {title : this.title}
      }
    }
  }
</script>
