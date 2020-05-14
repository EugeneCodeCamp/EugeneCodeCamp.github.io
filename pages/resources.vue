<template>
  <!-- Resources Section -->
  <section id="resources" class="page-section">
    <div class="container">
      <!-- Resources Section Heading -->
      <h2
        class="page-section-heading text-center text-uppercase text-secondary mb-0"
      >
        Resources
      </h2>

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
        <div class="col-md-12">
          <ul class="text-left">
            <li
              v-for="(resource, id) in resources"
              :key="id"
              class="list-group-item"
            >
              <a :href="resource.node.resource_url">
                {{ resource.node.title }}
              </a>
              - {{ resource.node.resource_description }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import axios from 'axios'
export default {
  asyncData() {
    return axios
      .post(`https://api.eugenecodecamp.com/graphql`, {
        query: `
            query MyQuery {
              resources {
                edges {
                  node {
                    id
                    resource_description
                    resource_url
                    slug
                    title
                  }
                }
              }
            }
            `
      })
      .then(res => {
        return { resources: res.data.data.resources.edges }
      })
  }
}
</script>

<style></style>
