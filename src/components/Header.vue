<template>
  <div class="container mx-auto">
    <div class="flex  mx-auto h-[92px] ">
      <div class="mx-10 my-8">
        <img src="/img/logo.png" alt="" />
      </div>
      <div class="mx-auto my-7 ">
        <ul class="gap-8 flex items-center mx-8">
          <router-link to="/home" class="[&.router-link-active]:text-white">Home</router-link>
                    <router-link to="/about" class="[&.router-link-active]:text-white text-slate-200">About us</router-link>
                    <router-link to="/pricing" class="[&.router-link-active]:text-white">Pricing</router-link>
                    <router-link to="/work" class="[&.router-link-active]:text-white">Work</router-link>
                    <router-link to="/blog" class="[&.router-link-active]:text-white">Blog</router-link>
        
        </ul>
      </div>
      <div>
        <button class="bg-[#1C1E53] text-white px-7 py-3 rounded-full border my-4 mx-8 hover:bg-white hover:text-[#1C1E53]">
          Contact Us
        </button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped></style>
