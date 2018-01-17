<template>
  <div class="hero">
    <h1 class="hero__title">
    {{ title }}
    <span class="hero__subtitle">{{ subtitle }}</span>
    </h1>
  </div>
</template>

<script>
export default {
  name: 'Hero',
  data () {
    return {
      title: 'Welcome to Impact Media!',
      subtitle: 'A Landing Page Built with VueJS'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hero {
  background-color: #5d5771;
  color: white;
  display: flex;
  justify-content: center;
  align-iten: center;
  text-align: center;
  font-weight: 300;
  padding: 8rem 0;
}

.hero__subtitle {
  display: block;
  font-weight: 300;
  font-size: 1.25rem;
}
</style>
