<script>
export default {
    name: "singleMovie",
    props: {
        details: Object
    }
}
</script>

<template>
    <div class="text-center">
        <img :src="details.poster_path" alt="#" class="mb-3">
        <h4>{{ details.original_title }}</h4>
        <div>{{ details.original_language }}</div>
        <div>{{ details.vote_average }}</div>

    </div>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables' as *;
</style>