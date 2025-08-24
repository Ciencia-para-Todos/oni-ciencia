<script>
    import Header from './components/Header.vue'
    import Body from './components/Body.vue'
    import Index from './components/Index.vue'
    import AuthorInfo from './components/AuthorInfo.vue'

    export default {
        components: {
            Header,
            Body,
            Index,
            AuthorInfo
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
    <header class="header-container">
            <Header />
    </header>
    <div class="page-container">
        <div class="left-side-container">
            <Index />
        </div>
        <div class="body-container">
            <Body />
        </div>
        <div class="right-side-container">
            <AuthorInfo />
        </div>
    </div>
</template>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    :root {
        /* Color variables */
        --grayish-white: #EFEFEF;
        --apricot: #ffd6c0;
        --melon: #FFA5A5;
        --deep-pink: #EC368D;
        --indigo: #440381;
        --electric-blue: #51E5FF;

        /* Property variables */
        --header-height: 4rem;
    }
    body {
        background-color: var(--apricot);
        margin: 0;
        font-family: "Montserrat";
        width: 100dvw;
    }
    .header-container {
        display: flex;
        z-index: 1000;
        top: 0;
        position: fixed;
    }
    .page-container {
        display: flex;
        width: inherit;
        margin-top: var(--header-height);
        flex-direction: row;
        justify-content: space-around;
    }
    .left-side-container,
    .right-side-container {
        display: flex;
        align-items: center;
        z-index: 999;
        position: fixed;
        height: calc(100dvh - 64px);
        width: 22dvw;
    }   
    .left-side-container {
        left: 0;
    }
    .right-side-container {
        right: 0;
    }
    .body-container {
        display: flex;
        z-index: 999;
        position: absolute;
        width: 56dvw;
        justify-content: center;
    }
    @media (max-width: 450px) {
        .left-side-container,
        .right-side-container {
            visibility: hidden;
        }
        .body-container {
            width: 100dvw;
        }
    }
</style>
