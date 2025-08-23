<script>
    import Header from './components/Header.vue'

    export default {
        components: {
            Header
        },
        data() {
            return {
                activePage: 0,
                pages: [
                    {
                        link: { text: 'Home', url: 'index.html'},
                        pageTitle: 'Início',
                    }
                ]
            }
        },
    }
</script>

<template>
    <Header />
</template>

<style scoped>

</style>
