<script>
    
</script>

<template>
    <nav class="navbar-container">
        <ul class="page-selector">
            <li class="selector" id="home-select">
                <button class="btn-select">
                    <span class="text-select">
                        Início
                    </span>
                </button>
            </li>
        </ul>
        <div class="profile-container">
            <a class="profile-picture" href="">
                <img class="profile-picture" src="../assets/OniCiência_v0.png" alt="Emblema de perfil.">
            </a>
        </div>
    </nav>
</template>

<style scoped>
    .navbar-container {
        display: flex;
        height: 64px;
        width: 100dvw;
        background-color: black;
    }
    .page-selector {
        width: 25%;
        height: 32px;
        padding: 0 16px;
        /*
        display: flex;
        justify-content: center;
        align-items: center;
        */
        align-content: center;
    }
    .profile-container {
        display: flex;
        align-content: center;
        align-items: center;
    }
    .profile-picture {
        border-radius: 32px;
        width: 48px;
        height: 48px;
    }
</style>