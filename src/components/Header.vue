<template>
  <div class="container">
    <div class="flex justify-between items-center h-[92px]">
      <div class="my-8">
        <img src="/img/logo.png" alt="" class="w-24 md:w-auto " />
      </div>
      <div class="md:hidden">
        <button @click="toggleMenu" class="focus:outline-none">
          <svg
            class="w-8 h-8 text-gray-700"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16m-7 6h7"
            ></path>
          </svg>
        </button>
      </div>
      <div class="hidden md:flex my-7  ">
        <ul class="gap-8 flex">
          <router-link
            to="/home"
            class="[&.router-link-active]:text-white hover:text-white text-gray-400"
            >Home</router-link
          >
          <router-link
            to="/about"
            class="[&.router-link-active]:text-white hover:text-white text-gray-400"
            >About us</router-link
          >
          <router-link
            to="/pricing"
            class="[&.router-link-active]:text-white hover:text-white text-gray-400"
            >Pricing</router-link
          >
          <router-link
            to="/work"
            class="[&.router-link-active]:text-white hover:text-white text-gray-400"
            >Work</router-link
          >
          <router-link
            to="/blog"
            class="[&.router-link-active]:text-white hover:text-white text-gray-400"
            >Blog</router-link
          >
        </ul>
      </div>
      <div class="hidden md:block">
        <router-link
          @click="closeMenu"
          to="/Contact"
          class="[&.router-link-active]:text-white bg-[#1C1E53] text-white px-7 py-3 rounded-full border my-4 mx-8 hover:bg-white hover:text-[#1C1E53]"
          >Contact Us
        </router-link>
      </div>
    </div>
    <div v-if="menuOpen" class="md:hidden">
      <ul class="flex flex-col items-center bg-[#1C1E53] shadow-md py-4">
        <router-link
          @click="closeMenu"
          to="/home"
          class="py-2  hover:text-white text-gray-400"
          >Home</router-link
        >
        <router-link
          @click="closeMenu"
          to="/about"
          class="py-2 hover:text-white text-gray-400"
          >About us</router-link
        >
        <router-link
          @click="closeMenu"
          to="/pricing"
          class="py-2  hover:text-white text-gray-400"
          >Pricing</router-link
        >
        <router-link
          @click="closeMenu"
          to="/work"
          class="py-2 hover:text-white text-gray-400"
          >Work</router-link
        >
        <router-link
          @click="closeMenu"
          to="/blog"
          class="py-2 hover:text-white text-gray-400"
          >Blog</router-link
        >
        <router-link
          @click="closeMenu"
          to="/Contact"
          class="[&.router-link-active]:text-white bg-[#1C1E53] text-white  py-3 rounded-full border my-4 hover:bg-white hover:text-[#1C1E53]"
          >Contact Us
        </router-link>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const menuOpen = ref(false);

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};

const closeMenu = () => {
  menuOpen.value = false;
};
</script>

<style scoped></style>
