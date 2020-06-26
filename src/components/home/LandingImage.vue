<template>
  <div class="landingimage">
    <v-img src="http://placekitten.com/g/800/600" contain />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class LandingImage extends Vue {}
</script>

<style scoped lang="scss">
.landingimage {
  width: 100vw;
  height: 80vh;
  background-color: red;
}
</style>
