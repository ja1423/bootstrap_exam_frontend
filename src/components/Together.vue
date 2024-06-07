<template>
  <div class="container lg:mx-auto mb-12">
    <div class="py-10  gap-6 ">
      <div class="mx-auto ">
        <h2 class="text-3xl font-bold max-w-[500px] text-center my-6">
          Let's build someting great together
        </h2>
        <p class="max-w-[500px] text-center my-12">
          Nullam vitae purus at tortor mattis dapibus. Morbi purus est,
          ultricies nec dolor sit amet, scelerisque cursus purus.
        </p>
      </div>
      <div class="max-md:flex justify-center md:mx-28">
        <router-link
          to="/Contact"
          class="[&.router-link-active]:text-white hover:text-gray-400 border bg-yellow-300 rounded-full py-4 px-8"
        >
          Contact Us
        </router-link>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped></style>
