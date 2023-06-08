<script>
export default {
    name: 'AppHeader',
    props: ['message'],
}
</script>


<template>
    <header class="container">
        <h1 class="text-center my-5">
            {{ message }}
        </h1>
        <input type="text" placeholder="Inserisci il titolo di un film">
        <input type="text" placeholder="prova">
        <button>Cerca</button>
    </header>
</template>


<style scoped lang="scss">
h1 {
    font-weight: 700;
}
</style>
