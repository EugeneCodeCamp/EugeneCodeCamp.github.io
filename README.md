# [Eugene Code Camp](https://eugenecodecamp.com/)

Welcome to Eugene Code Camp. The purpose of this site is to share coding meet up opportunities in the Eugene, Oregon area, and coding resources. All are welcome. Please refer to the [Contributing](https://github.com/EugeneCodeCamp/EugeneCodeCamp.github.io/blob/master/CONTRIBUTING.md) and [Code of Conduct](https://github.com/EugeneCodeCamp/EugeneCodeCamp.github.io/blob/master/CODE_OF_CONDUCT.md) documents for more information about participating in this repo.


This site is an ongoing project, currently being built in [Vue.js](https://vuejs.org/), using [Nuxt.js](https://nuxtjs.org/) and [Boostratp-vue](https://bootstrap-vue.js.org/), styled using the [Freelancer Theme from Start-Bootstrap](https://github.com/BlackrockDigital/startbootstrap-freelancer).

## Getting Started


### install dependencies
    $ npm install

### serve with hot reload at localhost:3000
    $ npm run dev

### build for production and launch server
    $ npm run build
    $ npm run start

### generate static project
    $ npm run generate

## Linting

### Prior to pushing files, please run
    $ npm run lint
    $ npm run lintfix

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## Database

For funsies, this site has an associated headless WordPress stack which serves as an API for REST or GraphQL.

### General Endpoints

* [REST Endpoint](https://api.eugenecodecamp.com/wp-json/wp/v2/)
* [GraphQL Endpoint](https://api.eugenecodecamp.com/graphql)

### Resources Data

* [REST Endpoint for Resources](https://api.eugenecodecamp.com/wp-json/wp/v2/resources/)
* GraphQL - use main endpoint

The resources are labeled with tags for categorization, and feature these five pieces of data for each resource:
* link (url) `resource_url`
* title `title`
* tags (slugs) `termSlugs(taxonomies: TAG)` / `tags` > `slug`
* description `resource_description`
* slug `slug`

Sample GraphQL query to pull all available resources

```
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
```

Sample GraphQL query to pull alld available resources and their associated tags

```
query MyQuery {
  resources {
    edges {
      node {
        resource_description
        resource_url
        slug
        title
        termSlugs(taxonomies: TAG)
      }
    }
  }
}
```

Sample GraphQL query to pull all available tags for resources

```
query MyQuery {
  resources {
    edges {
      node {
        tags {
          edges {
            node {
              slug
            }
          }
        }
      }
    }
  }
}
```

Sample GraphQL query to pull all available resources for a specific tag `html`

```
query MyQuery {
  resources {
    edges {
      node {
        tags(where: {slug: "html"}) {
          edges {
            node {
              resources {
                nodes {
                  resource_description
                  resource_url
                  slug
                  title
                }
              }
            }
          }
        }
      }
    }
  }
}
```

### Documentation and Testing

* [WPGraphQL](https://docs.wpgraphql.com/)
* [GraphQL Query Tool](https://lucasconstantino.github.io/graphiql-online/)