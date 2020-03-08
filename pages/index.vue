<template>
  <div >
    <!-- Masthead -->
  <div class="masthead bg-primary text-white text-center">
    <div class="container d-flex align-items-center flex-column">

      <!-- Masthead Avatar Image -->
      <img class="masthead-avatar mb-5" src="~/assets/codecircle.svg" alt="">

      <!-- Masthead Heading -->
      <h1 class="masthead-heading text-uppercase mb-0">Eugene Code Camp</h1>

      <!-- Icon Divider -->
      <div class="divider-custom divider-light">
        <div class="divider-custom-line"></div>
        <div class="divider-custom-icon">
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="divider-custom-line"></div>
      </div>

      <!-- Masthead Subheading -->
      <p class="masthead-subheading font-weight-light mb-0">Want to learn code? Looking for support? Let's do this!</p>

    </div>
  </div>

  <!-- Portfolio Section -->
  <section class="page-section portfolio" id="events">
    <div class="container">

      <!-- Portfolio Section Heading -->
      <h2 class="page-section-heading text-center text-uppercase text-secondary mb-0">Coming Up!</h2>

      <!-- Icon Divider -->
      <div class="divider-custom">
        <div class="divider-custom-line"></div>
        <div class="divider-custom-icon">
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="divider-custom-line"></div>
      </div>

      <!-- Portfolio Grid Items -->
      <div class="row">

        <!-- Portfolio Item 1 -->
        <div class="col-md-6 col-lg-4">
          <div class="portfolio-item mx-auto" data-toggle="modal" data-target="#portfolioModal1">
            <div class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100">
              <div class="portfolio-item-caption-content text-center text-white">
                <font-awesome-icon :icon="['fas', 'plus']" size="3x"/>
              </div>
            </div>
            <h3 class="align-items-center justify-content-center h-100 w-100">
              <font-awesome-icon :icon="['fas', 'user-friends']"/>
               2/2 Eugene Code Camp Meetup</h3>
          </div>
        </div>

        <!-- Portfolio Item 2 -->
        <div class="col-md-6 col-lg-4">
          <div class="portfolio-item mx-auto" data-toggle="modal" data-target="#portfolioModal2">
            <div class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100">
              <div class="portfolio-item-caption-content text-center text-white">
                <font-awesome-icon :icon="['fas', 'plus']" size="3x"/>
              </div>
            </div>
            <h3 class="align-items-center justify-content-center h-100 w-100">
              <font-awesome-icon :icon="['fas', 'user-friends']"/>
            3/1 Eugene Code Camp Meetup</h3>
          </div>
        </div>

        <!-- Portfolio Item 3 -->
        <div class="col-md-6 col-lg-4">
          <div class="portfolio-item mx-auto" data-toggle="modal" data-target="#portfolioModal3">
            <div class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100">
              <div class="portfolio-item-caption-content text-center text-white">
                <font-awesome-icon :icon="['fas', 'plus']" size="3x"/>
              </div>
            </div>
            <h3 class="align-items-center justify-content-center h-100 w-100">
              <font-awesome-icon :icon="['fas', 'user-friends']"/>
               4/5 Eugene Code Camp Meetup</h3>
          </div>
        </div>

      </div>
      <!-- /.row -->

    </div>
  </section>

  <!-- About Section -->
  <section class="page-section bg-primary text-white mb-0" id="about">
    <div class="container">

      <!-- About Section Heading -->
      <h2 class="page-section-heading text-center text-uppercase text-white">Who are we?</h2>

      <!-- Icon Divider -->
      <div class="divider-custom divider-light">
        <div class="divider-custom-line"></div>
        <div class="divider-custom-icon">
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="divider-custom-line"></div>
      </div>

      <!-- About Section Content -->
      <div class="row">
        <div class="col-lg-4 ml-auto">
          <p class="lead">Greg McKelvey is a web developer for <a href="https://www.twentyideas.com" class="text-secondary">Twenty Ideas</a>, a local Eugene tech company. Greg used <a href="https://www.freecodecamp.org" class="text-secondary">FreeCodeCamp.org</a> to change careers from teaching high school to coding. Still retaining his passion for teaching, he would be more than welcome to show you some of his favorite tools and resources that he used to bootstrap his new career in tech! (<a href="https://www.gatsbyjs.org" class="text-secondary">Gatsby</a> anyone?!)</p>
        </div>
        <div class="col-lg-4 mr-auto">
          <p class="lead">Nikole Garcia is a WordPress Engineer for <a href="https://x-team.com" class="text-secondary">X-Team</a>, an Australia-based developer-centric company with remote staff all over the world. She loves everything server-side, but will occasionally make her way frontward. Nikole brings over two decades of professional web development experience to our code camp meetups &mdash; but she'd say she's always still learning.</p>
        </div>
      </div>

      <!-- About Section Button -->
      <div class="text-center mt-4">
        <a class="btn btn-xl btn-outline-light" href="https://www.meetup.com/EugeneTech/events/265735915/">
          <font-awesome-icon :icon="['fab', 'meetup']" />
          Join Us!
        </a>
      </div>

    </div>
  </section>

  <!-- Resources Section -->
  <section class="page-section" id="resources">
    <div class="container">

      <!-- Resources Section Heading -->
      <h2 class="page-section-heading text-center text-uppercase text-secondary mb-0">Resources</h2>

      <!-- Icon Divider -->
      <div class="divider-custom">
        <div class="divider-custom-line"></div>
        <div class="divider-custom-icon">
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="divider-custom-line"></div>
      </div>

      <!-- Find Us Section -->
      <div class="row">
        <div class="col-md-6 col-lg-4">
          <ul>
            <li><a href="https://www.freecodecamp.org">freeCodeCamp</a> - Responsive web design, javascript, front end libraries, data visualization, information security and more!</li>
            <li><a href="https://www.codecademy.com">Codecademy</a> - HTML, CSS, Python, JavaScript, SQL, Ruby, PHP and more!</li>
            <li><a href="https://www.theodinproject.com">The Odin Project</a> - tracks for Full Stack Ruby on Rails, Full Stack JS, and Front End Only</li>
            <li><a href="https://www.udemy.com/the-web-developer-bootcamp/">The Web Developer Bootcamp</a> - HTML, CSS, JS, Node, and More!</li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Learn">Mozilla Development Network</a> - HTML, CSS, JS documentation, examples, and tutorials!</li>
            <li><a href="https://fullstackopen.com">Full Stack Open 2019</a> - Learn React, Redux, Node.js, MongoDB, and GraphQL in one go! This course will introduce you to modern JavaScript-based web development. The main focus is on building single page applications with ReactJS that use REST APIs built with Node.js.</li>
            <li><a href="https://www.100daysofcode.com/">100 Days of Code</a> - Commit to 100 Days of Code!</li>
          </ul>
        </div>
        <div class="col-md-6 col-lg-4">
          <ul>
            <li>Udemy Courses by Jonas Schmedtmann (low cost bootcamp-style classes from a top teacher):
              <ul>
                <li><a href="https://www.udemy.com/design-and-develop-a-killer-website-with-html5-and-css3/">Build Responsive Real World Websites with HTML5 and CSS3</a></li>
                <li><a href="https://www.udemy.com/advanced-css-and-sass/">Advanced CSS and Sass: Flexbox, Grid, Animations and More!</a></li>
                <li><a href="https://www.udemy.com/the-complete-javascript-course/">The Complete JavaScript Course 2019: Build Real Projects!</a></li>
                <li><a href="https://www.udemy.com/nodejs-express-mongodb-bootcamp/">Node.js, Express, MongoDB &amp; More: The Complete Bootcamp 2019</a></li>
                <li><a href="https://www.udemy.com/course/web-design-secrets/">Web Design for Web Developers: Build Beautiful Websites!</a></li>
              </ul>
            </li>
            <li><a href="https://www.edx.org/course/cs50s-introduction-to-computer-science">CS50 at Harvard University</a> - An introduction to the intellectual enterprises of computer science and the art of programming.</li>
          </ul>
        </div>
        <div class="col-md-6 col-lg-4">
          <ul>
            <li>Eugene-Area Coding Meetups:
              <ul>
                <li><a href="http://eugenewebdevs.com">Eugene Web Devs</a> - A monthly meetup for those interested in web development.</li>
                <li><a href="https://www.meetup.com/Elm-Eug/">Elm Eugene / Funky Ducks</a> - For everything functional programming! (Also a fun and educational Friday lunch hangout.)</li>
                <li><a href="https://www.meetup.com/pyeugene/">PyEugene</a> - A monthly meetup for those interested in the Python programming language.</li>
                <li><a href="https://www.meetup.com/Eugene-Area-SQL-Server-User-Group/">Eugene Area SQL Server User Group</a> - An official PASS chapter monthly meetup for SQL Server users.</li>
                <li><a href="https://www.meetup.com/Technology-Association-of-Oregon-in-greater-Eugene/">Eugene ISSA</a> - A monthly presentation for cybersecurity professionals and students.</li>
                <li><a href="https://www.meetup.com/Corvallis-WordPress-Meetup/">Corvallis WordPress Meetup</a> - A group of local WordPress developers, designers, and publishers who get together to share knowledge and experience.</li>
                <li><a href="https://www.meetup.com/Eugene-Cybersecurity/">Eugene Cybersecurity</a> - A meetup to talk IT Cybersecurity and related issues.</li>
              </ul>
            </li>
          </ul>
        </div>
      </div>

    </div>
  </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import { library } from '@fortawesome/fontawesome-svg-core'
import { faStar, faPlus, faUserFriends } from '@fortawesome/free-solid-svg-icons'
import { faMeetup } from '@fortawesome/free-brands-svg-icons'

export default {
  components: {
    Logo
  }
}
</script>

<style>
</style>
