<template>
        <div>
          <label :for="id" class="form-label m-2">{{label}}</label>
            <input
                :id="id"
                :type="type"
                :placeholder="placeholder"
                :class="inputClass"
            />
        </div>
</template>
  
<script>
    export default {
        name: 'AlloyInput',
        props: {
            id: String,
            label: String,
            type: String,
            placeholder: String,
            inputClass: String,
        },
        methods: {
            formOutput(e) {
                this.$emit('clicked',e )
            }
        }
    }
</script>
  
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
  