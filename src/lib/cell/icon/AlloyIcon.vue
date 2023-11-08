<template>
  <span :class="iconClass">
    <font-awesome-icon :icon="icon" />
  </span>
</template>

<script>
export default {
  name: 'AlloyIcon',
  props: {
    icon: String,
    iconClass: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
