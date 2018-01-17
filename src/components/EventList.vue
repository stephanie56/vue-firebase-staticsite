<template>
  <section class="event-list">
    <h2 class="section__title">Current Events</h2>
    <div class="event-list__item" v-for="event in events">
      <img class="event-list__thumbnail" :src="event.img" />
      <div>
        <span class="event-list__date">{{ event.date }}</span>
        <h3 class="event-list__name">{{ event.name }}</h3>
        <p class="event-list__description">{{ event.description }}</p>
        <Button />
      </div>
    </div>
  </section>
</template>

<script>
import Button from './Button'

export default {
  name: 'EventList',
  data () {
    return {
      events: [
        {
          name: 'VueJS 101',
          date: 'July 5th, 2018',
          start: '2:00pm',
          img: 'https://coligo.io/dynamic-components-in-vuejs/cover.jpg',
          description: 'This is a workshop for beginners to learn how to get started with VueJS.'
        },
        {
          name: 'Webpack for the Fun',
          date: 'July 12th, 2018',
          start: '6:00pm',
          img: 'http://www.dotnetcurry.com/images/angularjs/angular2-webpack/angular-with-webpack.png',
          description: 'We will build customize webpack config together. Don\'t forget to bring your laptop!'
        }
      ]
    }
  }
}
</script>

<style>
  section {
    padding: 3rem 0;
  }

  .section__title {
    font-size: 2rem;
    text-align: center;
    color: #5d5771;
    margin-bottom: 4rem;
  }

  .event-list__item{
    padding-bottom: 4rem;
    display: flex;
    max-width: 800px;
    margin: 0 auto;
  }

  .event-list__thumbnail {
    width: 200px;
    height: 150px;
    margin-right: 2rem;
    border: 1px solid #e3e3e3;
  }

  .event-list__name {
    font-size: 1.8rem;
  }
</style>
