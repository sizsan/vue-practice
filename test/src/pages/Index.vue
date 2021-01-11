<template>
  <q-page class="flex flex-center">
    <h1>{{title}}</h1>
    <p>{{text}} {{getTime}}</p>
    <Icon name="warning"/>
  </q-page>
</template>
<script>
import Icon from 'components/Icon'
export default {
  name: 'PageIndex',
  components: {
    Icon
  },
  data () {
    return {
      title: 'Hello World',
      text: 'Wow look at you go',
      date: null
    }
  },
  created () {
    setInterval(() => {
      this.date = Date()
    }, 1000)
  },
  computed: {
    getTime () {
      return this.date
    }
  },
  methods: {
    getDate () {
      return Date()
    }
  }
}
</script>
