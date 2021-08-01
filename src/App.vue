<template>
  <div>    
    <div>
      <!-- use this component to render each unique card. Hint:you should use v-for and v-bind here-->
      <BusinessCard />
    </div>
    <div>
      <!-- add the code to create a new business card here.-->
    </div>
  </div>
</template>

<script>
import BusinessCard from '@/components/BusinessCard.vue'
export default {
  components: {
    BusinessCard
  }, 
  data(){
    return{
      // maintain this data structure for your solution
      items: [
        {first_name: '', last_name: '', job_title: '', experience: 0, email: '', phone: 0},
      ]
    }
  },
  methods: {
    newCard(){
        return
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
html{
  background-color: #fafafa
}
</style>
