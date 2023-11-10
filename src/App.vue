<template>
  <AlloyInput
    id = "input1"
    label="Input 1"
    type="text"
    placeholder="Input 1"
    inputClass="form-control m-2"
  />
  <AlloyButtonIcon 
    id = "button1"
    icon="fa-solid fa-user-secret" 
    iconClass="btn btn-primary" 
    name="button1" 
    buttonClass="btn btn-primary m-2"
    @clicked="onClickChild"
/>
</template>

<script>
import AlloyButtonIcon from './lib/cell/button/ButtonIcon.vue'
import AlloyInput from './lib/input/AlloyInput.vue'

export default {
  name: 'App',
  components: {
    AlloyButtonIcon,
    AlloyInput
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
