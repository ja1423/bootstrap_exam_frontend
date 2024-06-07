<template>
    <div class="container ">
        <div>
            <h1 class="text-center text-4xl font-semibold my-8">Contact Us</h1>
            <p class="text-center max-w-[500px] mx-auto text-sm text-gray-700">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p>
        </div>

          
       
  <div class="container  py-12">
    <div class="max-w-3xl mx-auto bg-gray-100 p-8 rounded-lg shadow-md">
      <h1 class="text-center text-2xl font-semibold mb-6">Contact Us</h1>
      <form class="space-y-6" @submit.prevent="submitForm">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div>
            <label for="name" class="block text-sm font-medium text-gray-700">Name</label>
            <input type="text" id="name" v-model="formData.name" placeholder="Enter your name" required class="mt-1 block w-full border-gray-300 shadow-sm sm:text-sm rounded-md py-2 px-3 focus:none">
          </div>
          <div>
            <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
            <input type="email" id="email" v-model="formData.email" placeholder="Enter your Email" required class="mt-1 block w-full border-gray-300 shadow-sm sm:text-sm rounded-md py-2 px-3">
          </div>
          <div>
            <label for="subject" class="block text-sm font-medium text-gray-700">Subject</label>
            <input type="text" id="subject" v-model="formData.subject" placeholder="Provide context" required class="mt-1 block w-full border-gray-300 shadow-sm sm:text-sm rounded-md py-2 px-3">
          </div>
          <div>
            <label for="selectSubject" class="block text-sm font-medium text-gray-700">Subject</label>
            <input type="text" id="selectSubject" v-model="formData.selectSubject" placeholder="Select Subject" required class="mt-1 block w-full border-gray-300 shadow-sm sm:text-sm rounded-md py-2 px-3">
          </div>
        </div>
        <div>
          <label for="message" class="block text-sm font-medium text-gray-700">Message</label>
          <textarea id="message" v-model="formData.message" placeholder="Write your question here" required class="mt-1 block w-full border-gray-300 shadow-sm sm:text-sm rounded-md h-32 px-3 py-3"></textarea>
        </div>
        <div class="flex justify-center">
          <button type="submit" class="py-2 px-6 border border-transparent shadow-sm text-sm font-medium rounded-md text-white bg-gray-800 hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500">
            Send Message
          </button>
        </div>
      </form>
    </div>
  </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const formData = ref({
  name: '',
  email: '',
  subject: '',
  selectSubject: '',
  message: ''
});

const submitForm = () => {
  // Handle form submission logic here
  console.log('Form submitted:', formData.value);
};
</script>

<style scoped>
/* Add any custom styles here */
</style>

       
