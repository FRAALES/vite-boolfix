<script>
import axios from 'axios';
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader
  }
}
</script>

<template>
  <AppHeader message="BoolFlix" />
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
