<template>
   <div>
      <h1>Side bar</h1>
  <nuxt />
   </div>
   </template>

<script>

export default {
   components: {

   },
   props: {
      hoge: {
         type: Array,
         default: () => []
      }
   },
   data() {
      return {
         
      };
   },
   computed: {
      
   },
   methods: {

   }
}
</script>

<style scoped>
.app {
   width: 100%;
   height: 100%;
}
</style>