<template>
  <div>
    <div class="header">
      <div class="logo">
        <img src="~assets/img/jamstack-full-logo.svg" />
        <span>Norge</span>
      </div>
      <nav>
        <nuxt-link to="blogg">Blogg</nuxt-link>
        <a 
          href="https://www.meetup.com/JAMstack-Oslo/" 
          target="_blank"
        >Meetup</a>
        <nuxt-link to="about">Om</nuxt-link>
        <nuxt-link to="kontakt">Kontakt</nuxt-link>
      </nav>
    </div>
    <nuxt/>
  </div>
</template>

<style lang="scss">
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

div.header {
  display: flex;
  justify-content: flex-end;
  justify-content: space-between;
  div.logo {
    margin: 12px;
    span {
      font-size: 28px;
      font-weight: 100;
      font-style: italic;      
    }
  }
  nav {
    //margin-right: 10px;
    margin-right: 35px;
    margin-top: 20px;
    a {
      margin: 10px;
      text-decoration: none;
      color: #333;
    }
  }
}
</style>
