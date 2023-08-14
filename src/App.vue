<template>
  <div id="app" class="app-container">
    <landing-page></landing-page>
  </div>
</template>

<script>
import LandingPage from './LandingPage.vue'

export default {
  components: {
    LandingPage
  }
}
</script>

<style>
.app-container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  margin: 0;
  padding: 0;
  background-color: #ffffff; /* Same soft red background color */
}
</style>

