<template>
  <div class="frontpage">
    <section class="whatSection">
      <h2>Hva er Jamstack ?</h2>
      <p>Moderne webutvikling arkitektur basert på JavaScript, APIer og Markup</p>
    </section>
    <section class="whySection">
      <h2>Hvorfor Jamstack ?</h2>
      <ul>
        <li>Bedre ytelse</li>
        <li>Høyere sikkerhet</li>
        <li>Enklet å skalere</li>
        <li>Moderne utviklingsmiljø</li>
      </ul>
    </section>
    <!-- Latest -->
    <section class="latestBlogPosts">
      <h2>Seneste innlegg</h2>
      <div class="previewBlog">
        <!-- Bilde -->
        <h3>Hvorfor og hvordan migrere fra WordPress ?</h3>
        <h5>Av: <nuxt-link to="forfatter">Aman Mender</nuxt-link></h5>
      </div>
    </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
  }
}
</script>

<style lang="scss">
section {
  padding: 5% 5% 5% 5%;
  text-align: center;  
  color: white;
  h2 {
    font-weight: normal;
    text-align: left;
    margin-bottom: 20px;
  }
  p {
    font-size: 1.4em;
    padding: 20px 20%;
    color: #333;
    margin-bottom: 20px;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding-left: 0; 
    padding: 20px 0;
    li {
      flex: 1;
      font-size: 1.4em;
      flex: 1 0 50%;
      margin: 20px 0;
    }
  }
  &.whatSection {
    background: #63a5be;
    //background: url('~assets/img/pattern_1.svg'), linear-gradient(#63a5be,#63a5be);
    //background: linear-gradient(#63a5be,#63a5be);
  }
  &.whySection {
    background: #1da01d;
  }
  &.latestBlogPosts {
    h2 {
      color: #333;
    }
    div.previewBlog {
      text-align: left;
      color: #333;
      h3 {
        font-weight: normal;
      }
      h5 {
        font-weight: normal;
        a {
          text-decoration: none;
          color: #333;
        }
      }
    }
  }
}
</style>
