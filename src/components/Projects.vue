<template>
  <div class="container ">
    <div class="my-12">
      <div class="md:flex justify-between mb-6 ">
        <h2 class="text-3xl ">View our projects</h2>
        <div class="flex gap-3 ">
          <button class="">View More</button>
          <svg class="my-3"
            xmlns="http://www.w3.org/2000/svg"
            width="1em"
            height="1em"
            viewBox="0 0 16 16"
          >
            <path
              fill="black"
              fill-rule="evenodd"
              d="M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
      </div>

      <div class="md:grid grid-cols-3 gap-5">
    <div class="col-span-2 row-span-2 relative overflow-hidden group">
      <img class="w-full h-full" src="/img/card1.png" alt="" />
      <div
        class="absolute bg-gradient-to-br from-[#1C1E536B]/40 to-[#1C1E53] top-0 w-1/2 md:-left-full h-full text-white md:group-hover:left-0 duration-1000"
      >
        <div class="flex flex-col gap">
          <div class="max-md:hidden max-w-[400px] h-[400px]"></div>
          <div class="max-w-1/2 text-left md:px-9 ">
            <h3 class="md:text-2xl font-semibold mb-4">
              Workhub office Webflow Webflow Design
            </h3>
            <p class="text-white/80 mb-10 max-md:text-xs">
              Euismod faucibus turpis eu gravida mi. Pellentesque et velit
              aliquam
            </p>
            <router-link
              class="flex items-center max-md:text-sm md:gap-x-4 gap-2 cursor-pointer text-[#FCD980]"
              to="/pricing"
              >View Pricing
              <svg
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
      </div>
    </div>
    <div class="relative overflow-hidden group">
      <img class="w-full h-full" src="/img/card2.png" alt="" />
      <div
        class="absolute  bg-gradient-to-br from-[#1C1E536B]/40 to-[#1C1E53] top-0 md:group-hover:w-full md:w-1/2 w-full -left-full h-full text-white group-hover:left-0 duration-1000"
      >
        <div class="flex flex-col">
          <div class="w-60 md:h-32 h-20"></div>
          <div>
            <h3 class="text-2xl font-semibold mb-4 max-w-48">
              Unisaas Website Design
            </h3>
            <router-link
              class="flex items-center gap-x-4 cursor-pointer text-[#FCD980]"
              to="/pricing"
              >View Pricing
              <svg
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
      </div>
    </div>
    <div class="relative overflow-hidden group">
      <img class="w-full h-full" src="/img/card3.png" alt="" />
      <div
        class="absolute  bg-gradient-to-br from-[#1C1E536B]/40 to-[#1C1E53] top-0 group-hover:w-full w-1/2 -left-full h-full text-white group-hover:left-0 duration-1000"
      >
        <div class="flex flex-col">
          <div class="w-60 md:h-40 h-20"></div>
          <div>
            <h3 class="text-2xl font-semibold mb-8 max-w-48">
              Unisaas Website Design
            </h3>
            <router-link
              class="flex items-center gap-x-4 cursor-pointer text-[#FCD980] mb-6"
              to="/pricing"
              >View Pricing
              <svg
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
      </div>
    </div>
  </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
