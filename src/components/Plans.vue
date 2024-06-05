<template>
  <div class="container mx-auto">
    <div class="py-12">
      <div>
        <h1 class="font bold text-4xl text-center">Our Pricing Plans</h1>
        <p class="text-sm max-w-[700px] text-center mx-auto text-slate-700">
          When you’re ready to go beyond prototyping in Figma, Webflow is ready
          to help you bring your designs to life — without coding them.
        </p>
      </div>

      <div class="flex">
        <div class="rounded-lg  px-8 mx-2 my-12 bg-[#F4F6FC] hover:shadow-xl">
          <div class="flex gap-8 px-6 py-8">
            <h1 class="font-bold text-2xl">$299</h1>
            <p class="text-[#2405F2]">Per Design</p>
          </div>
          <div class="px-7 gap-8">
            <h1 class="font-semibold text-lg">Landing Page</h1>
            <p class="text-[#282938] text-sm max-w-[300px] my-4">
              When you’re ready to go beyond prototyping in Figma,
            </p>
            <div class="py-8 gap-4">
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p>All limited links</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p>Own analytics platform</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p>Chat support</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer1.svg" alt="" />
                <p>Optimize hashtags</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer1.svg" alt="" />
                <p>Unlimited users</p>
              </div>
            </div>

            <div class="justify-center mx-auto">
              
                <router-link
          to="/Home"
          class="[&.router-link-active]:text-white border bg-[#282938] rounded-full px-8 py-4 text-white hover:bg-white hover:text-[#282938]"
        >Get started
        </router-link>
            </div>
          </div>
        </div>

         <div class="rounded-lg px-8 mx-2 my-12 bg-[#1C1E53] hover:shadow-xl">
          <div class="flex gap-8 px-6 py-8">
            <h1 class="font-bold text-2xl text-white">$399</h1>
            <p class="text-[#FCD980] ">Multi Design</p>
          </div>
          <div class="px-7 gap-8">
            <h1 class="font-semibold text-lg text-white">Website Page </h1>
            <p class="text-[#FFFFFF] text-sm max-w-[300px] my-4">
              When you’re ready to go beyond prototyping in Figma, Webflow’s ready to help.
            </p>
            <div class=" gap-4">
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p class="text-white">All limited links</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p class="text-white">Own analytics platform</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p class="text-white">Chat support</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p class="text-white">Optimize hashtags</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p class="text-white">Unlimited users</p>
              </div>
            </div>

            <div class="justify-center mx-auto my-12">
              
              <router-link
          to="/Home"
          class="[&.router-link-active]:text-white border bg-[#FCD980] rounded-full px-8 py-4 text-white hover:bg-white hover:text-[#282938]"
          >Get started</router-link
        >
            </div>
          </div>
        </div>

         <div class="rounded-lg  px-8 mx-2 my-12 bg-[#F4F6FC] hover:shadow-xl">
          <div class="flex gap-8 px-6 py-8">
            <h1 class="font-bold text-2xl ">$499 +</h1>
            <p class="text-[#1C1E53] ">Per Design</p>
          </div>
          <div class="px-7 gap-8">
            <h1 class="font-semibold text-lg">Complex Project </h1>
            <p class="text-[#282938] text-sm max-w-[300px] my-4">
              When you’re ready to go beyond prototyping in Figma,
            </p>
            <div class=" gap-4">
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p >All limited links</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p >Own analytics platform</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p >Chat support</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p >Optimize hashtags</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p >Unlimited users</p>
              </div>
              <div class="flex gap-4 py-3">
                <img src="/icons/pointer.svg" alt="" />
                <p>Assist and Help</p>
              </div>
            </div>

            <div class="justify-center mx-auto my-4 mb-12 ">
              <router-link
          to="/Contact"
          class="[&.router-link-active]:text-white hover:text-gray-400 border bg-[#282938] rounded-full py-3 px-8 text-white"
          >Contact Us</router-link
        >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped></style>
