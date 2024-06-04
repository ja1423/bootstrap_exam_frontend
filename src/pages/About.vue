<template>
<div  class=" bg-[#1C1E53]" >
  <Header/>
</div>
    <div>
        <About />
        <Goals />
    </div>


<div class="bg-[#F4F6FC]">
<Team />
</div>


     <div class=" bg-[#1C1E53]">
        <Footer />
      </div>
</template>

<script setup lang="ts">
import About from "../components/About.vue"
import Header from "../components/Header.vue"
import Footer from "../components/Footer.vue"
import Goals from "../components/Goals.vue"
import Team from "../components/Team.vue"



</script>

<style scoped>

</style>