<script>
import { store } from './store.js';
import axios from 'axios';
import AppHeader from './components/AppHeader.vue'
import movieList from './components/movieList.vue'

export default {
  components: {
    AppHeader,
    movieList
  },
  data() {
    return {
      store,
    }
  },
  methods: {
    getMovies() {
      axios
        .get(store.apiURL)
        .then(res => {
          store.movieList = res.data.original_title;
        })
        .catch(err => {
          console.log(err);
        })
    }
  },
  created() {
    this.getMovies();
  }
}
</script>

<template>
  <AppHeader message="BoolFlix" />
  <movieList />
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
