<template>
    <div  class=" bg-[#1C1E53] sticky top-0 left-0 z-40" >
  <Header/>
</div>


<div class="bg-[#F4F6FC]">
<Portfolio />
</div>



<div>
    <Portfolios />
    <Together />
</div>


<div class=" bg-[#1C1E53]">
        <Footer />
      </div>
</template>

<script setup>
    import Header from "../components/Header.vue";
    import Footer from "../components/Footer.vue";
    import Portfolio from "../components/Portfolio.vue";
    import Portfolios from "../components/Portfolios.vue";
    import Together from "../components/Together.vue";
</script>

<style scoped>

</style>