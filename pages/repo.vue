<template>
    <header class="header">
        <NuxtLink to="/"><div class="menu"><p>accueil</p></div></NuxtLink>
        <NuxtLink to=""><div class="menu"><p>projets</p></div></NuxtLink>
        <NuxtLink to="contact"><div class="menu"><p>contact</p></div></NuxtLink>
    </header>
    <div class="mainBox">
        <div v-for="project in data" class="repo">
            {{project.name}}
        </div>
    </div>
    <footer class="footer">
        <a href="https://youtu.be/dQw4w9WgXcQ" target="_blank">
            Notilus11
        </a>
    </footer>
</template>

<script setup>
    const data = await $fetch('/api/hello');
    console.log(data[0].name)
</script>

<style scoped>
.menu{
    border-radius: 10px;
}
div.menu:hover{
    background-color: rgb(43, 49, 49);
    box-shadow: 0px 0px 5px rgb(0, 255, 225);
}
.repo {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border-radius: 5px;
    background-color: rgb(35, 35, 35);
    color: rgb(255, 255, 255);
    width: 30vw;
    height: 5vh;

}
.mainBox {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-image: url('https://wallpapercrafter.com/sizes/2560x1440/136245-Aperture-Laboratories-wall-texture-circle-digital-art-Portal-game-video-games.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-color: rgb(255, 255, 255);
    width: 100vw;
    height: 100vh;
}
.footer {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    text-decoration: underline;
    color: rgb(255, 150, 0);
    background-color: rgb(0, 0, 0);
    width: 100vw;
    height: 5vh;
}
</style>