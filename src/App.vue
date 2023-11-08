<template>
  <AlloyButtonIcon 
  id = "button1"
  icon="fa-solid fa-user-secret" 
  iconClass="btn btn-primary" 
  name="button1" 
  buttonClass="btn btn-primary mx-2"
  @clicked="onClickChild"
/>
<AlloyButtonIcon 
  id = "button2"
  icon="fa-solid fa-user-secret" 
  iconClass="btn btn-primary" 
  name="button2" 
  buttonClass="btn btn-primary mx-2"
  @clicked="onClickChild"
/>
<ol id="example-3">
<li v-for="item in itemslist" :key="item.id">
{{ item.message }}
</li>
</ol>
</template>

<script>
import AlloyButtonIcon from './lib/cell/button/ButtonIcon.vue'

export default {
  name: 'App',
  components: {
    AlloyButtonIcon
  },
  methods: {
    onClickChild (value) {
        alert(value) // someValue
    }
  },
  data() {
    return {
      itemslist: [
        { id: 1, message: 'Foo' },
        { id: 2, message: 'Bar' }
      ]
    }
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
