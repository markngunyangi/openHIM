<template>
  <div class="container">
    <Header title="Add a client"/>

    <Button name="Basic Info" color="green" @toggle="displayBasicInfo"/>
    <Button name="Authentication" @toggle="displayAuthentication"/>
    <component :is="currentComponent" v-if="currentComponent"></component>

  </div>
</template>


<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Button from '@/components/Button.vue'
import BasicInfo from '@/components/BasicInfo.vue'
import Authentication from '@/components/Authentication.vue'


export default {
  name: 'HomeView',
  components: {
    Header,
    Button,
    BasicInfo,
    Authentication,
  },

  data(){
    return{
      currentComponent: 'BasicInfo'
    }
  },

  methods: {
    displayBasicInfo() {
      this.currentComponent = 'BasicInfo'; 
    },
    displayAuthentication() {
      this.currentComponent = 'Authentication'; 
  }
}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Poppins', sans-serif;
}

.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}


</style>
