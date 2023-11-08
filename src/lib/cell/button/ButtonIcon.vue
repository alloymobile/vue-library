<template>
    <button type="button" :class="buttonClass" @click="onClickButton(id)">
        <AlloyIcon :icon="icon" :iconClass="iconClass"/>
        <span class="px-2">{{ name }}</span>
    </button>
</template>
  
  <script>
import AlloyIcon from '../icon/AlloyIcon.vue';

  export default {
    name: 'AlloyButtonIcon',
    props: {
        id: String,
        icon: String,
        iconClass: String,
        name: String,
        buttonClass: String,
    },
    components: { AlloyIcon },
    methods: {
     onClickButton(e) {
         this.$emit('clicked',e )
     }
  }
}
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  </style>
  