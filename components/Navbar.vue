<template>
  <b-navbar class="fixed-top" style="background-color: #272727">
    <b-container>
      <!-- Content here -->
      <b-navbar-nav>
        <b-navbar-brand href="https://www.jelly-party.com"
          ><h2 class="brand-name">Jelly Party</h2></b-navbar-brand
        >
      </b-navbar-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <a
          class="text-decoration-none"
          href="https://chrome.google.com/webstore/detail/jelly-party/aiecbkandfgpphpdilbaaagnampmdgpd"
          ><button
            style="font-size:1em"
            class="btn btn-primary mr-2 d-none d-sm-block custom-button"
          >
            Get the extension
          </button></a
        >
        <a
          class="text-decoration-none"
          href="https://www.patreon.com/jellyparty"
          ><button style="font-size: 1em" class="btn btn-primary custom-button">
            Support us on Patreon
          </button></a
        >
      </b-navbar-nav>
    </b-container>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style scoped>
.brand-name {
  color: white;
}

.brand-name:hover {
  transition: color 0.2s ease-in-out;
  color: red;
}
</style>
