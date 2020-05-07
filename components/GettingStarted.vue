<template>
  <b-container class="mt-5 mb-5 text-center">
    <h1 class="mb-5">Watching videos together has never been this easy.</h1>
    <b-row>
      <b-col lg class="center-hv"
        ><h3>
          1)
          <a
            href="https://chrome.google.com/webstore/detail/jelly-party/aiecbkandfgpphpdilbaaagnampmdgpd"
            >Get the extension in the Chrome Store.</a
          >
          It's free.
        </h3>
        <b-img
          src="~/assets/getting-started-download-extension.png"
          fluid
          alt="Fluid image"
        ></b-img>
      </b-col>
      <b-col lg class="center-hv"
        ><h3>2) Customize your avatar.</h3>
        <b-embed
          autoplay
          loop
          mute
          type="video"
          aspect="16by9"
          src="~/assets/getting-started-customize-appearance_minified.mp4"
        ></b-embed>
      </b-col>
    </b-row>
    <b-row>
      <b-col lg class="center-hv"
        ><h3>3) Browse to a video & start a party.</h3>
        <b-embed
          autoplay
          loop
          mute
          type="video"
          aspect="16by9"
          src="~/assets/getting-started-customize-appearance_minified.mp4"
        ></b-embed
      ></b-col>
      <b-col lg class="center-hv"
        ><h3>4) Share your magic link.</h3>
        <b-img
          style="max-height: 500px"
          width="auto"
          src="~/assets/getting-started-share-magic-link.png"
          fluid
          alt="Fluid image"
        ></b-img
      ></b-col>
    </b-row>
    <b-row>
      <b-col lg class="center-hv"
        ><h3 style="margin-bottom: 0px">5) Grant permissions.</h3>
        <small
          >Only if you're joining a party — this has to be done only once for
          every website Jelly-Party runs on.</small
        >
        <b-embed
          autoplay
          loop
          mute
          type="video"
          aspect="16by9"
          src="~/assets/getting-started-joining-a-party_minified.mp4"
        ></b-embed>
      </b-col>
      <b-col lg class="center-hv"
        ><h3>6) Enjoy the party. Chat with your friends.</h3>
        <b-img
          style="max-height: 500px"
          width="auto"
          src="~/assets/getting-started-chat-with-your-friends.jpg"
          fluid
          alt="Fluid image"
        ></b-img>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {}
</script>

<style scoped>
img,
video {
  height: 300px;
}

.center-hv {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 64px;
}
</style>
