<template>
  <div>
    <Header />
    <!-- Other components or content -->
  </div>
</template>

<script>
import Header from './Header.vue';

export default {
  name: 'Home',
  components: {
    Header
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap');

body {
  margin: 0;
  font-family: 'Open Sans', sans-serif;
}
</style>
