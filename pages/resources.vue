<template>
  <!-- Resources Section -->
  <section id="resources" class="page-section">
    <div class="container">
      <!-- Resources Section Heading -->
      <!-- <h2 class="page-section-heading text-center text-uppercase text-secondary mb-0">Resources</h2> -->
      <h2 class="page-section-heading">Resources</h2>

      <!-- Icon Divider -->
      <div class="divider-custom">
        <div class="divider-custom-line" />
        <div class="divider-custom-icon">
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="divider-custom-line" />
      </div>

      <!-- Find Us Section -->
      <div class="row">
        <div class="col-md-6 col-lg-4">
          <ul class="text-left">
            <li class="list-group-item">{{ resources }}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      resources: ''
    }
  },
  async mounted() {
    try {
      const response = await this.$axios.$post(
        'https://api.eugenecodecamp.com/graphql',
        {
          query: `
            query MyQuery {
              resources {
                edges {
                  node {
                    resource_description
                    resource_url
                    slug
                    title
                  }
                }
              }
            }
            `
        }
      )
      this.resources = response
    } catch (e) {
      console.log('err', e)
    }
  }
}
</script>

<style></style>
