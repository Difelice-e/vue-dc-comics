<template>
  <div id="app">
    <PageHeader />
    <PageMain />
    <PageBanner />
    <PageFooter />

  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue'
import PageMain from './components/PageMain.vue'
import PageBanner from './components/PageBanner.vue'
import PageFooter from './components/PageFooter.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageMain,
    PageBanner,
    PageFooter
  }
}
</script>

<style lang="scss">
* {
  padding: 0.5em;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
