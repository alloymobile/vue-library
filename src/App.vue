<template>
  <AlloyButtonIcon 
  icon="fa-solid fa-user-secret" 
  iconClass="btn btn-primary" 
  name="Click me" 
  buttonClass="btn btn-primary d-flex flex-column align-items-center"
  @enlarge-text="onEnlargeText"
/>
</template>

<script>
import AlloyButtonIcon from './lib/cell/button/ButtonIcon.vue'

export default {
  name: 'App',
  components: {
    AlloyButtonIcon
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
