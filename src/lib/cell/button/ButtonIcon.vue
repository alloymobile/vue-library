<template>
    <button type="button" :class="buttonClass" @click="myMethod" @mouseenter="myMethod">
        <AlloyIcon :icon="icon" :iconClass="iconClass"/>
        <span class="px-2">{{ name }}</span>
    </button>
</template>
  
  <script>
import AlloyIcon from '../icon/AlloyIcon.vue';

  export default {
    name: 'AlloyButtonIcon',
    props: {
        icon: String,
        iconClass: String,
        name: String,
        buttonClass: String,
    },
    components: { AlloyIcon },
    methods: {
    myMethod: function myMethod(ev) {
      alert('Button clicked!'+ev); 
    }
  }
}
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  </style>
  