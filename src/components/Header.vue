<script>

</script>

<template>
    <nav class="navbar-container">
        <ul class="page-selector">
            <li class="selector" id="home-select">
                <button class="btn-select">
                    <svg class="icon-select" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 640"><path fill="#ec368d" d="M341.8 72.6C329.5 61.2 310.5 61.2 298.3 72.6L74.3 280.6C64.7 289.6 61.5 303.5 66.3 315.7C71.1 327.9 82.8 336 96 336L112 336L112 512C112 547.3 140.7 576 176 576L464 576C499.3 576 528 547.3 528 512L528 336L544 336C557.2 336 569 327.9 573.8 315.7C578.6 303.5 575.4 289.5 565.8 280.6L341.8 72.6zM304 384L336 384C362.5 384 384 405.5 384 432L384 528L256 528L256 432C256 405.5 277.5 384 304 384z"/></svg>
                </button>
            </li>
        </ul>
        <div class="profile-container">
            <a class="profile-frame" href="">
                <img class="profile-picture" src="../assets/OniCiência_v0.png" alt="Emblema de perfil.">
            </a>
        </div>
    </nav>
</template>

<style scoped>
    .navbar-container {
        display: flex;
        position: fixed;
        height: 64px;
        width: 100dvw;
        background-color: var(--apricot);
    }
    .page-selector {
        width: 25%;
        height: 32px;
        padding: 0 16px;
        align-content: center;
    }
    .selector {
        text-decoration: none;
        list-style: none;
    }
    .profile-container {
        display: flex;
        align-content: center;
        align-items: center;
    }
    .profile-frame {
        border-color: var(--deep-pink);
        border-radius: 32px;
        border-width: 2px;
        border-style: solid;
        width: 48px;
        height: 48px;
    }
    .profile-picture {  
        border-radius: 32px;      
        width: inherit;
        height: inherit;
    }
    .btn-select  {
        width: 32px;
        height: 32px;
        padding: 0;
        background: transparent;
        border: none;
    }
    .btn-select {
        width: 32px;
        height: 32px;
        background: transparent;
    }
    .icon-select {
        height: 32px;
        width: 32px;
    }
</style>