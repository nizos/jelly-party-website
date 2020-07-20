<template>
  <b-container
    class="pt-5 pb-5 d-flex align-items-center justify-content-center"
  >
    <iframe
      src="https://docs.google.com/forms/d/e/1FAIpQLSctyAA2k9qoPpPeiNHYVaZ4I493tli3Lz78B2d4mDIF6VzErw/viewform?embedded=true"
      width="640"
      height="960"
      frameborder="0"
      marginheight="0"
      marginwidth="0"
      >Loading…</iframe
    >
    <!-- <h1 class="mt-5 mb-5 text-center">
      Leave us feedback
    </h1>
    <p>
      We're thankful for any kind of feedback we get. Please fill out the below
      form to let us know where we're doing good and where we can do better.
      Alternatively, simply shoot us an
      <a href="mailto:hi@jelly-party.com">email</a>.
    </p>
    <b-form @submit.stop.prevent="onSubmit">
      <b-form-group
        id="fieldset-2"
        :description="
          `How do you like Jelly Party? ${value10 > 0 ? `(${value10})` : ''}`
        "
        label="Rate Jelly Party"
        label-for="rating-10"
        :invalid-feedback="'Please rate us'"
        :valid-feedback="'Thanks!'"
        :state="ratingState"
      >
        <b-form-rating
          id="rating-10"
          v-model="value10"
          stars="10"
          required
          name="rating"
        ></b-form-rating>
      </b-form-group>
      <b-form-group
        id="fieldset-3"
        label="How did you hear about Jelly Party?"
        label-for="how-hear"
        :invalid-feedback="'Let us know how you heard about Jelly Party.'"
        :valid-feedback="'Thanks!'"
        :state="howHearState"
      >
        <b-form-select
          id="how-hear"
          v-model="selectedHowHear"
          :options="howHearOptions"
          required
        ></b-form-select>
      </b-form-group>
      <b-form-group
        id="fieldset-4"
        label="Anything else you would like us to tell about? (Request more streaming services here)"
        label-for="free-text-feedback"
      >
        <b-form-textarea
          id="free-text-feedback"
          v-model="feedbackText"
          placeholder="Enter something..."
          rows="
        3"
          max-rows="6"
        ></b-form-textarea>
      </b-form-group>
      <b-button type="submit" variant="primary">Submit feedback</b-button>
    </b-form> -->
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      value10: 0,
      selectedHowHear: null,
      feedbackText: '',
      howHearOptions: [
        { value: null, text: 'Please select an option' },
        { value: 'a', text: 'Friends & family' },
        { value: 'b', text: 'Social media' },
        { value: 'c', text: 'Search engine / Internet' },
        { value: 'd', text: 'Other' }
      ]
    }
  },
  computed: {
    ratingState() {
      return Boolean(this.value10)
    },
    howHearState() {
      return Boolean(this.selectedHowHear)
    },
    validInput() {
      return Boolean(this.value10) && Boolean(this.selectedHowHear)
    }
  },
  methods: {
    onSubmit() {
      if (this.validInput) {
      } else {
        alert('Please fill out the required data.')
      }
    }
  }
}
</script>
