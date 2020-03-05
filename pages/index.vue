<template>
  <div>
    <Home />
  </div>
</template>

<script>
import Home from "~/components/Home";
export default {
  name: "HomePage",

  components: {
    Home
  },
  head() {
    return {
      title: "Amimul Ihsan Mahdi || Android Developer From Bangladesh"
    };
  }
};
</script>
