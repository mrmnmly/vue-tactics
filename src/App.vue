<template>
  <div id="app">
    <router-view/>
    <ui-footer></ui-footer>
  </div>
</template>

<script>
import UiFooter from '@/components/generic/Footer'

export default {
  name: 'App',
  components: {
    UiFooter
  } 
}
</script>


<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Press+Start+2P');

#app {
  font-family: 'Press Start 2P', cursive, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
