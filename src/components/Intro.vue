<template>
  <div class="container">
    <div class="bg-[#1C1E53] flex flex-col lg:flex-row py-14 items-center justify-between">
      <div class="left_side gap-5  text-center lg:text-left">
        <h1 class="font-bold text-[32px] lg:text-[54px] text-white mb-6 max-w-[300px] lg:max-w-[450px]  lg:mx-0">
          Building stellar websites for early startups
        </h1>
        <p class="text-sm tracking-widest font-medium text-white max-w-[300px] lg:max-w-[500px]  lg:mx-0">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt.
        </p>
        <div class="flex flex-col lg:flex-row gap-5   mt-8  lg:items-start">
          <router-link
            class="hover:bg-[#FCD980] border border-[#FCD980] hover:text-[#1B1C2B] text-[#FCD980] py-2 lg:py-4  lg:px-14 rounded-full cursor-pointer w-full lg:w-auto text-center"
            to="/work"
          >
            View our work
          </router-link>
          <router-link
            class="flex items-center gap-x-4 cursor-pointer w-full lg:w-auto justify-center lg:justify-start text-white py-4"
            to="/pricing"
          >
            View Pricing
            <svg
              class="animate-pulse"
              xmlns="http://www.w3.org/2000/svg"
              width="1.5em"
              height="1.5em"
              viewBox="0 0 512 512"
            >
              <path
                fill="currentColor"
                d="m359.873 121.377l-22.627 22.627l95.997 95.997H16v32.001h417.24l-95.994 95.994l22.627 22.627L494.498 256z"
              />
            </svg>
          </router-link>
        </div>
      </div>

      <div class="right_side lg:px-10 mt-8 lg:mt-0">
        <img src="/img/intro.png" alt="" class="w-full h-auto lg:w-auto lg:h-full"/>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped></style>
