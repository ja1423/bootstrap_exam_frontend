<template>
    <div class="container mx-auto">
        <div>
            <h1 class="text-center text-4xl font-semibold my-8">Contact Us</h1>
            <p class="text-center max-w-[500px] mx-auto text-sm text-gray-700">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.</p>
        </div>

          <div></div>
       

    </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      subject: '',
      showResponse: false,
      response: ''
    };
  },
  methods: {
    submitForm() {
      // Simulating an API call with a setTimeout
      setTimeout(() => {
        // Perform your API request here
        // For demonstration purposes, we'll just set a response message
        this.response = `Email sent to ${this.email} with subject: ${this.subject}`;
        this.showResponse = true;

        // Reset form fields
        this.email = '';
        this.subject = '';
      }, 2000);
    }
  }
};
</script>

<style scoped>

</style>