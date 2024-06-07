<template>
  <div class="container">
    <div class="py-12">
      <div>
        <h1 class="font-bold text-4xl text-center">Our Pricing Plans</h1>
        <p class="text-sm max-w-[700px] text-center mx-auto text-slate-700">
          When you’re ready to go beyond prototyping in Figma, Webflow is ready
          to help you bring your designs to life — without coding them.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 justify-center gap-5">
        <div
          v-for="(plan, index) in plans"
          :key="index"
          class="rounded-lg my-12 hover:shadow-xl"
          :class="plan.bgClass"
          @mouseover="hover = index"
          @mouseleave="hover = -1"
        >
          <div class="flex gap-8  py-8">
            <h1 class="font-bold text-4xl" :class="plan.textColor">{{ plan.price }}</h1>
            <p :class="plan.subTextColor">{{ plan.designType }}</p>
          </div>
          <div class="px-7 gap-8">
            <h1 class="font-semibold text-lg" :class="plan.textColor">{{ plan.title }}</h1>
            <p :class="[plan.textColor, 'text-sm max-w-[300px] my-4']">{{ plan.description }}</p>
            <div class="gap-4">
              <div v-for="(feature, featureIndex) in plan.features" :key="featureIndex" class="flex gap-4 py-3">
                <img :src="feature.icon" alt="feature icon" />
                <p :class="plan.textColor">{{ feature.text }}</p>
              </div>
            </div>
            <div class="justify-center my-12">
              <router-link
                v-if="plan.buttonText === 'Get started'"
                :to="plan.buttonLink"
                class="[&.router-link-active]:text-white border rounded-full px-8 py-4"
                :class="plan.buttonClass"
              >
                {{ plan.buttonText }}
              </router-link>
              <router-link
                v-else
                :to="plan.buttonLink"
                class="[&.router-link-active]:text-white hover:text-black hover:bg-white  border rounded-full py-4 px-8"
                :class="plan.buttonClass"
              >
                {{ plan.buttonText }}
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const plans = [
  {
    price: '$299',
    designType: 'Per Design',
    title: 'Landing Page',
    description: 'When you’re ready to go beyond prototyping in Figma,',
    features: [
      { icon: '/icons/pointer.svg', text: 'All limited links' },
      { icon: '/icons/pointer.svg', text: 'Own analytics platform' },
      { icon: '/icons/pointer.svg', text: 'Chat support' },
      { icon: '/icons/pointer1.svg', text: 'Optimize hashtags' },
      { icon: '/icons/pointer1.svg', text: 'Unlimited users' }
    ],
    buttonText: 'Get started',
    buttonLink: '/Home',
    bgClass: 'bg-[#F4F6FC]',
    textColor: 'text-[#282938]',
    subTextColor: 'text-[#2405F2]',
    buttonClass: 'bg-[#282938] text-white hover:bg-white hover:text-[#282938]'
  },
  {
    price: '$399',
    designType: 'Multi Design',
    title: 'Website Page',
    description: 'When you’re ready to go beyond prototyping in Figma, Webflow’s ready to help.',
    features: [
      { icon: '/icons/pointer.svg', text: 'All limited links' },
      { icon: '/icons/pointer.svg', text: 'Own analytics platform' },
      { icon: '/icons/pointer.svg', text: 'Chat support' },
      { icon: '/icons/pointer.svg', text: 'Optimize hashtags' },
      { icon: '/icons/pointer.svg', text: 'Unlimited users' }
    ],
    buttonText: 'Get started',
    buttonLink: '/Home',
    bgClass: 'bg-[#1C1E53]',
    textColor: 'text-white',
    subTextColor: 'text-[#FCD980]',
    buttonClass: 'bg-[#FCD980] text-white hover:bg-white hover:text-[#282938]'
  },
  {
    price: '$499 +',
    designType: 'Per Design',
    title: 'Complex Project',
    description: 'When you’re ready to go beyond prototyping in Figma,',
    features: [
      { icon: '/icons/pointer.svg', text: 'All limited links' },
      { icon: '/icons/pointer.svg', text: 'Own analytics platform' },
      { icon: '/icons/pointer.svg', text: 'Chat support' },
      { icon: '/icons/pointer.svg', text: 'Optimize hashtags' },
      { icon: '/icons/pointer.svg', text: 'Unlimited users' },
      { icon: '/icons/pointer.svg', text: 'Assist and Help' }
    ],
    buttonText: 'Contact Us',
    buttonLink: '/Contact',
    bgClass: 'bg-[#F4F6FC]',
    textColor: 'text-[#282938]',
    subTextColor: 'text-[#1C1E53]',
    buttonClass: 'bg-[#282938] text-white hover:text-gray-400'
  }
];

let hover = -1;
</script>

<style scoped>
/* Add custom styles here if needed */
</style>
