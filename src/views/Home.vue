<template>
  <div class="home">
    <LandingImage />
  </div>
</template>

<script>
// @ is an alias to /src
import LandingImage from "@/components/home/LandingImage.vue";

export default {
  name: "Home",
  components: {
    LandingImage
  }
};
</script>
