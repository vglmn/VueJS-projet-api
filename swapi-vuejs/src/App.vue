<template>
  <div id="app">
    <header>
      <span>SWAPI</span>
    </header>
    <main>
      <img src="./assets/logo.png" alt="SWAPI PWA">
      <router-view></router-view>
    </main>
    <footer>
      <span>Realized thanks to <a href="https://swapi.co/documentation">SWAPI</a> and the example of <a href="https://swapi-pwa.now.sh">Finnian Anderson</a></span>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app',
  metaInfo: {
    title: 'SWAPI',
    meta: [
      { name: 'description', content: 'SWAPI', vmid: 'description' },
      { name: 'og:description', content: 'SW-API', vmid: 'og:description' }
    ]
  }
}
</script>

<style>
* {
  box-sizing: border-box;
}

html, body {
  padding: 0;
  margin: 0;
  width: 100%;
  height: 100%;
  font-size: 18px;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000000;
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
}

main {
  text-align: center;
  flex: 1 0 auto;
}

header, footer {
  background-color: rgb(0, 0, 0);
  color: #ffe600;
}

header, footer {
  font-size: 1.5em;
  padding: 0.5em 1em;
  min-height: 2em;
}

header span,
footer span {
  display: block;
  line-height: 1;
  letter-spacing: .02em;
  box-sizing: border-box;
}

footer {
  flex-shrink: 0;
  padding: 1em 1.5em;
  font-size: 1em;
  text-align: center;
}

footer span:first-of-type {
  margin-bottom: .5em;
}

footer a {
  color: #fff;
  font-weight: bold;
  text-decoration: none;
}

</style>
