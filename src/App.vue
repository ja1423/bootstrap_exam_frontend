<script setup>
import Header from "./components/Header.vue"
import Intro from "./components/Intro.vue"
</script>

<template>
  <div>
  <Header />
  <div class="container mx-auto">
      <div class="grid grid-cols-4 gap-x-7">
        <Categories class="max-w-screen-md col-span-1 max-md:hidden" />
        <Products class="col-span-3" />
        <Intro />
      </div>
    </div>
  </div>
 
</template>

<style scoped>

</style>
