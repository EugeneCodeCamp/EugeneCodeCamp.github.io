<template>
  <div>
    <!-- Masthead -->
    <div class="masthead bg-primary text-white text-center">
      <div class="container d-flex align-items-center flex-column">
        <!-- Masthead Avatar Image -->
        <img class="masthead-avatar mb-5" src="~/assets/codecircle.svg" alt />

        <!-- Masthead Heading -->
        <h1 class="masthead-heading text-uppercase mb-0">Eugene Code Camp</h1>

        <!-- Icon Divider -->
        <div class="divider-custom divider-light">
          <div class="divider-custom-line" />
          <div class="divider-custom-icon">
            <font-awesome-icon :icon="['fas', 'star']" />
          </div>
          <div class="divider-custom-line" />
        </div>

        <!-- Masthead Subheading -->
        <p class="masthead-subheading font-weight-light mb-0">
          Want to learn code? Looking for support? Let's do this!
        </p>
      </div>
    </div>

    <!-- Portfolio Section -->
    <section id="events" class="page-section portfolio">
      <div class="container">
        <!-- Portfolio Section Heading -->
        <h2
          class="page-section-heading text-center text-uppercase text-secondary mb-0"
        >
          Coming Up!
        </h2>

        <!-- Icon Divider -->
        <div class="divider-custom">
          <div class="divider-custom-line" />
          <div class="divider-custom-icon">
            <font-awesome-icon :icon="['fas', 'star']" />
          </div>
          <div class="divider-custom-line" />
        </div>

        <!-- Portfolio Grid Items -->
        <div class="row">
          <!-- Portfolio Items -->
          <div
            v-for="event in events"
            :key="event.id"
            class="col-md-6 col-lg-4"
          >
            <div
              v-b-modal="'EventModal' + event.id"
              class="portfolio-item mx-auto"
            >
              <EventModal :event="event" />
              <div
                class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100"
              >
                <div
                  class="portfolio-item-caption-content text-center text-white"
                >
                  <font-awesome-icon :icon="['fas', 'plus']" size="3x" />
                </div>
              </div>
              <h3 class="align-items-center justify-content-center h-100 w-100">
                <font-awesome-icon :icon="['fas', 'user-friends']" />
                {{ event.title }}
              </h3>
            </div>
          </div>
        </div>
        <!-- /.row -->
      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="page-section bg-primary text-white mb-0">
      <div class="container">
        <!-- About Section Heading -->
        <h2 class="page-section-heading text-center text-uppercase text-white">
          Who are we?
        </h2>

        <!-- Icon Divider -->
        <div class="divider-custom divider-light">
          <div class="divider-custom-line" />
          <div class="divider-custom-icon">
            <font-awesome-icon :icon="['fas', 'star']" />
          </div>
          <div class="divider-custom-line" />
        </div>

        <!-- About Section Content -->
        <div class="row">
          <div class="col-lg-4 ml-auto">
            <p class="lead">
              Greg McKelvey is a web developer for
              <a href="https://www.twentyideas.com" class="text-secondary"
                >Twenty Ideas</a
              >, a local Eugene tech company. Greg used
              <a href="https://www.freecodecamp.org" class="text-secondary"
                >FreeCodeCamp.org</a
              >
              to change careers from teaching high school to coding. Still
              retaining his passion for teaching, he would be more than welcome
              to show you some of his favorite tools and resources that he used
              to bootstrap his new career in tech! (
              <a href="https://www.gatsbyjs.org" class="text-secondary"
                >Gatsby</a
              >
              anyone?!)
            </p>
          </div>
          <div class="col-lg-4 mr-auto">
            <p class="lead">
              Nikole Garcia is a WordPress Engineer for
              <a href="https://x-team.com" class="text-secondary">X-Team</a>, an
              Australia-based developer-centric company with remote staff all
              over the world. She loves everything server-side, but will
              occasionally make her way frontward. Nikole brings over two
              decades of professional web development experience to our code
              camp meetups &mdash; but she'd say she's always still learning.
            </p>
          </div>
        </div>

        <!-- About Section Button -->
        <div class="text-center mt-4">
          <a
            class="btn btn-xl btn-outline-light"
            href="https://www.meetup.com/EugeneTech/events/265735915/"
          >
            <font-awesome-icon :icon="['fab', 'meetup']" />Join Us!
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import EventModal from '@/components/EventModal'
export default {
  components: {
    EventModal
  },
  data: function() {
    return {
      events: [
        {
          id: 1,
          title: '4/5 Eugene Code Camp Online Meetup',
          description:
            "We're going to try this online. Please be on your computer when we meet up, in case you need to share your screen! Tell the group what you're working on, get some ideas of what to do next, and we can all help each other get through this, whether 'this' is being stuck on the code or stuck in your house.",
          eventUrl: 'https://www.meetup.com/EugeneCodeCamp/events/269740499/'
        },
        {
          id: 2,
          title: '4/19 Eugene Code Camp Online Meetup',
          description:
            "We're going to try this online. Please be on your computer when we meet up, in case you need to share your screen! Tell the group what you're working on, get some ideas of what to do next, and we can all help each other get through this, whether 'this' is being stuck on the code or stuck in your house.",
          eventUrl: 'https://www.meetup.com/EugeneCodeCamp/events/269749792/'
        },
        {
          id: 3,
          title: '5/3 Eugene Code Camp Online Meetup',
          description:
            "We're going to try this online. Please be on your computer when we meet up, in case you need to share your screen! Tell the group what you're working on, get some ideas of what to do next, and we can all help each other get through this, whether 'this' is being stuck on the code or stuck in your house.",
          eventUrl: 'https://www.meetup.com/EugeneCodeCamp/events/269749796/'
        }
      ]
    }
  }
}
</script>

<style></style>
