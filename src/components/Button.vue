<template>
  <a class="btn" href="#">Learn More</a>
</template>

<script>
export default {
  name: 'Button',
  data () {
    return {
      msg: 'Learn more'
    }
  }
}
</script>

<style scoped>
  .btn {
    display: inline-block;
    text-decoration: none;
    padding: 0.4rem 1rem;
    border: #42b983 1px solid;
  }
</style>
