<template>
  <b-modal
    :id="'EventModal' + event.id"
    class="sm-secondary"
    tabindex="-1"
    aria-labelledby="EventModal"
    ok-only
    button-size="lg"
  >
    <div role="document">
      <div class="text-center">
        <div class="row justify-content-center">
          <div class="col-lg-8">
            <!-- Portfolio Modal - Title -->
            <h2
              class="portfolio-modal-title text-secondary text-uppercase mb-0"
            >
              {{ event.title }}
            </h2>
            <!-- Icon Divider -->
            <div class="divider-custom">
              <div class="divider-custom-line"></div>
              <div class="divider-custom-icon">
                <font-awesome-icon :icon="['fas', 'star']" />
              </div>
              <div class="divider-custom-line"></div>
            </div>
            <!-- Portfolio Modal - Text -->
            <p class="mb-5">{{ event.description }}</p>
            <p class="mb-5">
              <a :href="event.eventUrl" target="_new">More Information</a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </b-modal>
</template>

<script>
export default {
  props: {
    event: {
      type: Object,
      default: function() {
        return {
          id: 1,
          title: 'TBA',
          description: 'Check back soon for more events.',
          eventUrl: 'https://www.meetup.com/EugeneCodeCamp/events/'
        }
      }
    }
  }
}
</script>

<style></style>
