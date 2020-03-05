<template>
  <div class="app">
    <Navigation />
    <nuxt />
  </div>
</template>

<script>
import Navigation from "~/components/global/Navbar";
export default {
  components: {
    Navigation
  },
  data() {
    return {};
  }
};
</script>

