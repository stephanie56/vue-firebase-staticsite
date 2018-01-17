<template>
  <div id="app">
    <Header />
    <Hero />
    <EventList />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header'
import Hero from './components/Hero'
import EventList from './components/EventList'
import Footer from './components/Footer'


export default {
  name: 'App',
  components: {
    Header,
    Hero,
    EventList,
    Footer
  }
}
</script>

<style>
* {
 margin: 0;
 padding: 0;
}
.container {
  max-width: 1024px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
