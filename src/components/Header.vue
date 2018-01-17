<template>
  <header id="header">
    <div class="container">
      <div class="logo">Logo</div>
      <nav class="main-nav">
        <ul>
          <li v-for="item in navList"><a :href="item.url" >{{ item.name }}</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      navList: [
        {
          name: 'About',
          url: '#'
        },
        {
          name: 'Portfolio',
          url: '#'
        },
        {
          name: 'What We Do',
          url: '#'
        },
        {
          name: 'Contact',
          url: '#'
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo {
  width: 20%;
  font-size: 1.25rem;
  display: flex;
  justify-content: center;
  align-items: center;
}
nav {
  width: 60%;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
  padding: 1rem;
}
a {
  color: #42b983;
  text-decoration: none;
}

</style>
