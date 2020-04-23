<template>
  <b-navbar class="fixed-top" toggleable="sm" style="background-color: #272727">
    <b-container>
      <!-- Content here -->
      <b-navbar-toggle target="nav-collapse">
        <template v-slot:default>
          <b-icon icon="list" width="1.5em" height="1.5em"></b-icon>
        </template>
      </b-navbar-toggle>

      <b-navbar-nav>
        <b-navbar-brand href="https://www.jelly-party.com"
          ><h2 class="brand-name">Jelly Party</h2></b-navbar-brand
        >
      </b-navbar-nav>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <a
            class="text-decoration-none"
            href="https://chrome.google.com/webstore/detail/jelly-party/aiecbkandfgpphpdilbaaagnampmdgpd"
            ><button
              style="font-size:1em"
              class="btn btn-primary mr-2 custom-button mt-2 mb-2"
            >
              Get the extension
            </button></a
          >
          <a
            class="text-decoration-none"
            href="https://www.patreon.com/jellyparty"
            ><button
              style="font-size: 1em"
              class="btn btn-primary custom-button mt-2 mb-2"
            >
              Support us on Patreon
            </button></a
          >
        </b-navbar-nav>
      </b-collapse>
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
.navbar-light .navbar-toggler-icon {
  background: url('data:image/svg+xml,%3csvg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 30 30"%3e%3cpath stroke="rgba(255, 255, 255, 1)" stroke-linecap="round" stroke-miterlimit="10" stroke-width="2" d="M4 7h22M4 15h22M4 23h22"/%3e%3c/svg%3e') !important;
}
</style>
