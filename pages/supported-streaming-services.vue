<template>
  <b-container class="pt-5 pb-5">
    <h1 class="mt-5 mb-5 text-center">
      Supported streaming services
    </h1>
    <b-table striped hover :items="sortedData"></b-table>
    <p>
      Please head to our <a href="feedback">feedback site</a> if you would like
      to request more services.
    </p>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          streamingService: 'Netflix',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '✓'
        },
        {
          streamingService: 'DisneyPlus',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '✓'
        },
        {
          streamingService: 'Youtube',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '✓'
        },
        {
          streamingService: 'Vimeo',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '⨯'
        },
        {
          streamingService: 'Jellyfin',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '✓'
        },
        {
          streamingService: 'PrimeVideo',
          videoSynchronization: '✓',
          chat: '✓',
          fullscreen: '✓'
        }
      ]
    }
  },
  computed: {
    sortedData() {
      const streamingServiceNames = this.items.map(
        (item) => item.streamingService
      )
      streamingServiceNames.sort()
      const sortedData = []
      for (const streamingServiceName of streamingServiceNames) {
        sortedData.push(
          this.items.find(
            (item) => item.streamingService === streamingServiceName
          )
        )
      }
      return sortedData
    }
  }
}
</script>
