<script setup>
import Header from "./components/Header.vue"
import Intro from "./components/Intro.vue"
import Projects from "./components/Projects.vue"
import Features from "./components/Features.vue"
import Clients from "./components/Clients.vue"
</script>

<template>
  <div  class=" bg-[#1C1E53]" >
  <Header/>
  
        <Intro />
      </div>

      <div>
        <Projects />
        
      </div>

      <div class="bg-[#F4F6FC] ">
        <Features />
      </div>
 
 <div>
  <Clients />
 </div>

 
</template>

<style scoped>

</style>
