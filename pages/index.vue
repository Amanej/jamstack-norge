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
      //margin-bottom: 20px;
      margin-bottom: 40px;
    }
  }
}
section.whatSection {
  background: #63a5be;
}
section.whySection {
  background: #1da01d;
}
</style>
