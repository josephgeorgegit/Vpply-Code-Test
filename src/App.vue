<template>
  <div>
    <div v-if="showInstructions">
      <Instructions />
    </div>

      <button @click="showInstructions=!showInstructions"><span v-if="!showInstructions">Show</span><span v-if="showInstructions">Hide</span> instructions</button>

      <!-- Start writing your html here. Make sure to use at least 1 component -->
    <div>
      <div>
        <!-- use this component to render each unique card. Hint:you should use v-for and v-bind here-->
        <ListItem />
      </div>
      <div>
        <!-- add the code to create a new business card here. Hint: you should use v-model here-->
      </div>
    </div> 
  
  </div>
</template>

<script>
import Instructions from '@/components/Instructions.vue'
import ListItem from '@/components/ListItem.vue'
export default {
  components: {Instructions, ListItem},
  data(){
    return{
      showInstructions: true,
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
