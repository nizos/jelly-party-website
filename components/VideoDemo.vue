<template>
  <b-container fluid class="video-container">
    <b-row>
      <b-col
        xl="4"
        class="mt-5 d-flex align-items-center justify-content-center"
      >
        <h1 class="mt-2 mb-2 text-white text-center" style="max-width: 10em">
          Jelly-Party runs in your Chrome browser on Windows, macOs, ChromeOS
          &amp; Linux.
        </h1>
      </b-col>
      <b-col
        xl="8"
        class="mt-5 d-flex align-items-center justify-content-center mb-5 mt-5"
      >
        <video
          style="max-width: 1080px"
          autoplay
          loop
          src="~/assets/promo.webm"
          width="100%"
        ></video>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {}
</script>

<style scoped>
.video-container {
  background: linear-gradient(to bottom right, #9164ff 0%, #8bfff4 100%);
}
</style>
