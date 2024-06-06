<template>
    <div class="container mx-auto">
      <h3 class="text-[#282938] text-5xl leading-[64px] font-semibold text-center pt-[128px] pb-[48px]">Meet our team</h3>

      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 text-center pb-[128px]">
        <div v-for="(item, index) in team" :key="index">
          <div class="shadow-md bg-white relative overflow-hidden">
            <div class="flex justify-center   relative group my-6 mx-auto ">
              <img :src="item.img" :alt="`Photo of ${item.name}`" class="transition-opacity duration-300">
              <img class="absolute inset-0 opacity-0 group-hover:opacity-100 duration-300   px-[64px]  py-1 mx-auto " src="/img/team.png" alt="Overlay image">
              <div class="opacity-0 group-hover:opacity-100 duration-300 flex absolute inset-0 justify-center items-center gap-3 z-[20]">
                <img src="/icons/facebook.svg" alt="Facebook">
                <img src="/icons/twitter.svg" alt="Twitter">
                <img src="/icons/linkedin.svg" alt="LinkedIn">
              </div>
            </div>
            <div class="pb-[34px]">
              <p class="font-medium">{{ item.name }}</p>
              <p class="text-sm text-gray-500">{{ item.level }}</p>
            </div>
          </div>
        </div>
      </div>

    </div>
  
</template>

<script setup>
const team = [
  {
    img: '/img/man1.png',
    name: 'John Smith',
    level: 'CEO',
    hover: '/img/team.png',
  },
  {
    img: '/img/man2.png',
    name: 'Simon Adams',
    level: 'CTO',
    hover: '/img/team.png',
  },
  {
    img: '/img/man3.png',
    name: 'Paul Jones',
    level: 'Design Lead',
    hover: '/img/team.png',
  },
  {
    img: '/img/man4.png',
    name: 'Sara Hardin',
    level: 'Project Manager',
    hover: '/img/team.png',
  },
];
</script>

<style scoped>
/* Add custom styles here if needed */
</style>
