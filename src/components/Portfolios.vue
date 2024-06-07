<template>
  <div class="container mx-auto mb-12">
    <div>
      <div class="flex">
        <ul class="md:flex gap-6 mx-auto my-12">
          <li v-for="(category, index) in categories" :key="index">
            <a v-if="category.visible" :class="{ 'text-[#2405F2]': index === 0, 'text-sm text-gray-400 hover:text-[#2405F2]': index !== 0 }" :href="category.link">{{ category.name }}</a>
          </li>
        </ul>
      </div>
      <div class="md:grid grid-cols-2 gap-5">
        <div v-for="(template, index) in templates" :key="index">
          <img class=" py-5 w-full" :src="template.image" alt="" />
          <h1 class="text-3xl font-semibold py-5 ">{{ template.title }}</h1>
          <p class="text-gray-500 text-sm">{{ template.description }}</p>
          <div class="flex gap-2 hover:text-[#2405F2]">
            <button>{{ template.buttonText }}</button>
            <svg class="my-3" xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 16 16">
              <path fill="black" fill-rule="evenodd" :d="template.svgPath" clip-rule="evenodd" />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const categories = [
  { name: 'All', link: '#', visible: true },
  { name: 'UI Design', link: '#', visible: true },
  { name: 'Webflow Design', link: '#', visible: true },
  { name: 'Figma Design', link: '#', visible: true }
];

const templates = [
  { 
    image: '/img/img.png',
    title: 'Template 1',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'View Portfolio',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
  { 
    image: '/img/img2.png',
    title: 'Template 2',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'View Portfolio',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
  { 
    image: '/img/img3.png',
    title: 'Template 3',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'Read Case Study',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
  { 
    image: '/img/img4.png',
    title: 'Template 4',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'Read Case Study',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
  { 
    image: '/img/img5.png',
    title: 'Template 5',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'Read Case Study',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
  { 
    image: '/img/img6.png',
    title: 'Template 6',
    description: 'Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle.',
    buttonText: 'Read Case Study',
    svgPath: 'M10.159 10.72a.75.75 0 1 0 1.06 1.06l3.25-3.25L15 8l-.53-.53l-3.25-3.25a.75.75 0 0 0-1.061 1.06l1.97 1.97H1.75a.75.75 0 1 0 0 1.5h10.379z'
  },
];
</script>
