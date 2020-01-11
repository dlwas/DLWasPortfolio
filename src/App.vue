<template>
  <div id="app">
    <nav class="nav">
      <a href="https://www.froenda.com" class="nav__brand">FROENDA</a>
    </nav>
    <section>
      <p>COMING</p>
      <p>SOON</p>
    </section>
  </div>
</template>

<script>
  export default {
    name: 'app',
  }
</script>

<style lang="scss">
  @import '@/_media.scss';
  @import url('https://fonts.googleapis.com/css?family=Montserrat:700|Noto+Sans:700&display=swap');
  /* font-family: 'Noto Sans', sans-serif; */
  /* font-family: 'Montserrat', sans-serif; */

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    letter-spacing: 0.04em;
  }

  html {
    background: #121212;
  }

  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #ffffff;
    width: 90%;
    height: calc(100vh - 4rem);
    margin: 0px auto;
  }

  .nav {
    width: 100%;
    height: 4rem;
    margin: 0px auto;
    padding: 0px 24px;
    display: flex;
    align-items: center;

    &__brand {

      &:hover,
      &:visited,
      &:link,
      &:active {
        text-decoration: none;
        color: #ffffff;
      }

      font-family: 'Noto Sans',
      sans-serif;
      /* font-size: 1rem; */
      font-size: 14px;
      line-height: 19px;
      font-weight: bold;
    }
  }

  section {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
    height: 100%;
    margin: 0px auto;

    p {
      padding-top: -4rem;
      padding: 10px 10px;
      font-family: 'Montserrat', sans-serif;
      font-style: normal;
      font-weight: bold;
      font-size: 8rem;
      line-height: 78px;
      letter-spacing: 0.04em;
      text-transform: uppercase;
      color: #dbdbdb;
      text-shadow: 2px 2px 3px rgba(255, 182, 70, 0.25),
        -2px -2px 3px rgba(255, 182, 70, 0.25),
        -2px 2px 3px rgba(255, 182, 70, 0.25),
        2px -2px 3px rgba(255, 182, 70, 0.25);
    }

    p {
      @include breakpoint(fullhd) {
        font-size: 10rem;
        padding: 2rem 10px;
      }
    }

    p {
      @include breakpoint(desktop) {
        font-size: 8rem;
        padding: 1.5rem 10px;
      }
    }

    p {
      @include breakpoint(mobile) {
        font-size: 4.75rem;
        padding: 0.5rem 10px;
      }
    }

    p {
      @include breakpoint(mobilemin) {
        font-size: 4rem;
        padding: 0rem 10px;
      }
    }

  }
</style>