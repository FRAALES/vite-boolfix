<script>
import { store } from './../store.js';

import singleMovie from './singleMovie.vue';

export default {
    name: "movieList",
    components: {
        singleMovie
    },
    data() {
        return {
            store,
        }
    }
}
</script>


<template>
    <section class="container">

        <singleMovie v-for="movie in store.movieList" :details="movie" />

    </section>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables' as *;
</style>