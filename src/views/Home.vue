<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data(){
    return{
      property:'This is my property',
      propertyTwo:'2nd property'
    }
  },
  beforeCreate(){
    console.log("BeforeCreate()")
  },
  created(){
    console.log("Created()")
  },
  beforeMount(){
    console.log("BeforeMount()")
  },
  mounted(){
    console.log("Mounted()")
  },
  beforeDestroy(){
    console.log("BeforeDestroy()")
  },
  destroyed(){
    console.log("Destroyed()")
  }
}
</script>
