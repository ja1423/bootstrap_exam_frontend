<template>
    <div class="container mx-auto">
        <div class="md:flex mx-7">
            <div>
                <h1 class="text-4xl max-w-[500px] font-bold mb-4">Frequently asked questions</h1>
                <router-link
          to="/Contact"
          class="[&.router-link-active]:text-white  text-[#2405F2] "
          >Contact us For More Info</router-link
        >
        </div>

  <div class="md:w-[1400px] pb-10 mx-8 w-full">
    <div
      v-for="(data, index) in datas"
      :key="index"
      class="relative mb-10 py-4 border-b-2 cursor-pointer"
      @click="toggleInfo(index)"
    >
      <div class="md:flex  gap-7 mb-5">
        <span class="text-2xl text-[#2405F2]">0{{ index + 1 }}</span>
        <h3 class="md:text-2xl text-xl max-md:w-[200px]">
          {{ data.question }}
        </h3>
        <span
          v-if="!data.isVisible"
          class="absolute right-10 text-2xl text-[#2405F2]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="0.88em"
            height="1em"
            viewBox="0 0 448 512"
          >
            <path
              fill="currentColor"
              d="M256 80c0-17.7-14.3-32-32-32s-32 14.3-32 32v144H48c-17.7 0-32 14.3-32 32s14.3 32 32 32h144v144c0 17.7 14.3 32 32 32s32-14.3 32-32V288h144c17.7 0 32-14.3 32-32s-14.3-32-32-32H256z"
            />
          </svg>
        </span>
        <span
          v-if="data.isVisible"
          class="absolute right-10 text-2xl text-[#2405F2]"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="1em"
            height="1em"
            viewBox="0 0 24 24"
          >
            <g fill="none" fill-rule="evenodd">
              <path
                d="M24 0v24H0V0zM12.593 23.258l-.011.002l-.071.035l-.02.004l-.014-.004l-.071-.035c-.01-.004-.019-.001-.024.005l-.004.01l-.017.428l.005.02l.01.013l.104.074l.015.004l.012-.004l.104-.074l.012-.016l.004-.017l-.017-.427c-.002-.01-.009-.017-.017-.018m.265-.113l-.013.002l-.185.093l-.01.01l-.003.011l.018.43l.005.012l.008.007l.201.093c.012.004.023 0 .029-.008l.004-.014l-.034-.614c-.003-.012-.01-.02-.02-.022m-.715.002a.023.023 0 0 0-.027.006l-.006.014l-.034.614c0 .012.007.02.017.024l.015-.002l.201-.093l.01-.008l.004-.011l.017-.43l-.003-.012l-.01-.01z"
              />
              <path
                fill="currentColor"
                d="m12 14.122l5.303 5.303a1.5 1.5 0 0 0 2.122-2.122L14.12 12l5.304-5.303a1.5 1.5 0 1 0-2.122-2.121L12 9.879L6.697 4.576a1.5 1.5 0 1 0-2.122 2.12L9.88 12l-5.304 5.304a1.5 1.5 0 1 0 2.122 2.12z"
              />
            </g>
          </svg>
        </span>
      </div>
      <p
        v-show="data.isVisible"
        class="duration-1000 text-lg leading-8 text-primary/80 md:pl-[70px] pl-14 max-w-[650px] "
      >
        {{ data.answer }}
      </p>
    </div>
  </div>
 </div>
            </div>
  
</template>

<script setup>
import { ref } from "vue";

const datas = ref([
  {
    question: "How much time does it take ?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    isVisible: false,
  },
  {
    question: "What is your class naming convention ?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    isVisible: false,
  },
  {
    question: "How do we communicate ?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    isVisible: false,
  },
  {
    question: "I have a bigger project. Can you handle it ?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    isVisible: false,
  },
  {
    question: "What is your class naming convention ?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    isVisible: false,
  },
]);

const toggleInfo = (index) => {
  datas.value[index].isVisible = !datas.value[index].isVisible;
};
</script>

<style lang="scss" scoped>
/* Add any scoped styles you need here */
</style>
      

