<template>
  <b-modal
    id="portfolioModal1"
    class="portfolio-modal modal fade bg-secondary"
    tabindex="-1"
    role="dialog"
    aria-labelledby="portfolioModal1Label"
  >
    <div class="modal-dialog modal-xl" role="document">
      <div class="modal-content">
        <div class="modal-body text-center">
          <div class="row justify-content-center">
            <div class="col-lg-8">
              <!-- Portfolio Modal - Title -->
              <h2
                class="portfolio-modal-title text-secondary text-uppercase mb-0"
              >
                4/5 Eugene Code Camp Online Meetup
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
              <p class="mb-5">
                We're going to try this online. Please be on your computer when
                we meet up, in case you need to share your screen! Tell the
                group what you're working on, get some ideas of what to do next,
                and we can all help each other get through this, whether "this"
                is being stuck on the code or stuck in your house.
              </p>
              <p class="mb-5">
                <a
                  href="https://web.cvent.com/event/f2e9191c-6323-4e80-bb0b-c080002ac037/summary"
                  target="_new"
                  >More Information</a
                >
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </b-modal>
</template>

<script>
export default {}
</script>

<style></style>
