<template>
  <div id="app">
    <nav>
      <h1 class="brand-name">FROENDA</h1>
    </nav>
    <div class="section">
      <p>COMING</p>
      <p>SOON<span>.</span><span>.</span><span>.</span></p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app',
  }
</script>

<style>
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

  nav {
    width: 100%;
    height: 4rem;
    margin: 0px auto;
    padding: 0px 24px;
    display: flex;
    align-items: center;
  }

  .brand-name {
    font-family: 'Noto Sans', sans-serif;
    /* font-size: 1rem; */
    font-size: 14px;
    line-height: 19px;
    font-weight: bold;
  }

  .section {
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 100%;
    height: 100%;
    margin: 0px auto;
  }

  p {
    padding-top: -4rem;
    /* display: block; */
    padding: 0 10px;
    font-family: 'Montserrat', sans-serif;
    font-style: normal;
    font-weight: bold;
    font-size: 64px;
    line-height: 78px;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: rgba(255, 182, 70, 0.64);
  }

.section span {
    animation-name: blink;
    animation-duration: 1.4s;
    animation-iteration-count: infinite;
    animation-fill-mode: both;
}

.section span:nth-child(2) {
    animation-delay: .2s;
}

.section span:nth-child(3) {
    animation-delay: .4s;
}

  @keyframes blink {
    0% {
      opacity: .2;
    }

    20% {
      opacity: 1;
    }

    100% {
      opacity: .2;
    }
  }
</style>