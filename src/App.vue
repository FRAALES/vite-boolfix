<script>
import { store } from './store.js';
import axios from 'axios';
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader
  },
  data() {
    return {
      store,
    }
  }
}
</script>

<template>
  <AppHeader message="BoolFlix" />
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
