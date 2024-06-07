<template>
    <div  class=" bg-[#1C1E53] sticky top-0 left-0 z-40" >
  <Header/>
</div>


<Plans />
<Questions />


<div class=" bg-[#1C1E53]">
        <Footer />
      </div>
</template>

<script setup>
    
    import Header from "../components/Header.vue"
    import Footer from "../components/Footer.vue"
    import Plans from "../components/Plans.vue"
    import Questions from "../components/Questions.vue"

</script>

<style scoped>

</style>