<template>
  
    <h3>{{ title }}</h3>

</template>

<script>
export default {
  name: 'Header',
  props: {
    title: String
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

</style>
