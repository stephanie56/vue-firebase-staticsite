<template>
  <footer>
    <div class="container">
      {{ copyright }}
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data () {
    return {
      copyright: `© ${new Date().getFullYear()} Impact Media. All Rights Reserved.`
    }
  }
}
</script>

<style >
  footer {
    background-color: #42b983;
    color: white;
    padding: 1.25rem 0;
    display: flex;
    align-item: center;
    justify-content: center;
  }
</style>
