<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div class="container">
     <button type="button" class="btn btn-success">Success</button>
     <button type="button" class="btn btn-info">Info</button>
     <button type="button" class="btn btn-warning">Warning</button>
  </div>
  <font-awesome-icon :icon="icon" />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    icon: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
