<template>
  <div class="container mx-auto">
    <div class="flex flex-col md:flex-row py-24 px-8 ">
      <div class="md:w-1/2">
        <div class="gap-5 mx-12 my-12">
          <h1 class="text-3xl font-semibold">What our clients say about us</h1>
          <p class="text-[#282938] text-sm max-w-[300px] py-4">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit sed.
          </p>
        </div>
      </div>
      <div class="md:w-1/2 mt-8 md:mt-0">
        <div class="swiper-container overflow-hidden">
          <div class="swiper-wrapper">
            <div v-for="item in 3" :key="item" class="swiper-slide">
              <h2 class="font-semibold text-3xl max-w-[800px]">
                "The best agency we’ve worked with so far. They understand our product
                and are able to add new features with a great focus."
              </h2>
              <div class="flex justify-between items-center mt-4">
                <div class="flex gap-4">
                  <img class="py-12 " src="/img/jenny.png" alt="" />
                  <div class="my-10">
                    <h1 class="font-semibold text-xl">Jenny Wilson</h1>
                    <p>Vice President</p>
                  </div>
                </div>
                <div class="flex gap-4">
                  <button @click="goToPrevSlide" class="rounded-full border py-5 my-8 px-6 hover:bg-[#5239FA] text-[#5239FA]">
                    <svg
                      width="13"
                      height="22"
                      viewBox="0 0 13 22"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        opacity="0.6"
                        d="M11.5859 -1.23626e-07L13 3.21951L3.96947 10.9106L13 18.7805L11.5859 22L9.06922e-07 11.626L1.06329e-06 9.8374L11.5859 -1.23626e-07Z"
                        fill="#282938"
                      />
                    </svg>
                  </button>
                  <button @click="goToNextSlide" class="rounded-full border px-6 py-5 my-8 hover:bg-[#5239FA] text-[#5239FA]">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="1em"
                      height="1em"
                      viewBox="0 0 1024 1024"
                    >
                      <path
                        fill="black"
                        d="M338.752 104.704a64 64 0 0 0 0 90.496l316.8 316.8l-316.8 316.8a64 64 0 0 0 90.496 90.496l362.048-362.048a64 64 0 0 0 0-90.496L429.248 104.704a64 64 0 0 0-90.496 0"
                      />
                    </svg>
                  </button>
                </div>
              </div>
            </div>
          </div>
          <!-- Add pagination -->
          <div class="swiper-pagination"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper';
import 'swiper/swiper-bundle.css';

export default {
  mounted() {
    // Initialize Swiper
    this.swiper = new Swiper('.swiper-container', {
      loop: true,
      pagination: {
        el: '.swiper-pagination',
      },
    });
  },
  methods: {
    goToPrevSlide() {
      this.swiper.slidePrev();
    },
    goToNextSlide() {
      this.swiper.slideNext();
    },
  }
};
</script>

<style>
/* Custom styles can be added here */
</style>
