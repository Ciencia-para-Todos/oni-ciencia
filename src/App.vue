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

<style>
    :root {
        --apricot: #ffd6c0;
        --melon: #FFA5A5;
        --deep-pink: #EC368D;
        --indigo: #440381;
        --electric-blue: #51E5FF;
    }
    body {
        margin: 0;
    }
</style>
