<template>
  <div class="bg-[#1C1E53] sticky top-0 left-0 z-40">
    <Header />
  </div>

  <Contact />

  <div class="bg-[#1C1E53]">
    <Footer />
  </div>
</template>

<script setup>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";
import Contact from "../components/Contact.vue";
</script>

<style scoped></style>
