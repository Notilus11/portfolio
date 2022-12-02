<template>
    <header class="header">
        <NuxtLink to="/"><div class="menu"><p>accueil</p></div></NuxtLink>
        <NuxtLink to="repo"><div class="menu"><p>projets</p></div></NuxtLink>
        <NuxtLink to=""><div class="menu"><p>contact</p></div></NuxtLink>
    </header>
    <div class="mainBox">
        <a href="https://instagram.com/yann_malaret?igshid=YmMyMTA2M2Y=" target="_blank">
            <div class="reseau">
                    <img class="img" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/640px-Instagram_icon.png"
                    width="120">
            </div>
        </a>
        <a href="https://github.com/Notilus11?tab=repositories" target="_blank">
            <div class="reseau">
                    <img class="img" src="https://cdn-icons-png.flaticon.com/512/25/25231.png"
                    width="120">
            </div>
        </a>
        <div class="reseau">
                <img class="img" src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/Twitter-logo.svg/2491px-Twitter-logo.svg.png"
                width="120">
        </div>
    </div>
    <footer class="footer">
        <a href="https://youtu.be/dQw4w9WgXcQ" target="_blank">
            yann.malaret@outlook.fr
        </a>
    </footer>
</template>

<style scoped>
.menu{
    border-radius: 10px;
}
div.reseau:hover{
    background-color: rgb(78, 78, 78);
    height: 210px;
    width: 210px;
}
div.menu:hover{
    background-color: rgb(43, 49, 49);
    box-shadow: 0px 0px 5px rgb(0, 255, 225);
}
.reseau {
    border: 1px solid rgb(255, 150, 0);
    box-shadow: 10px 7px 10px rgb(0, 0, 0);
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    background-color: rgb(63, 61, 61);
    width: 200px;
    height: 200px;
}
.mainBox {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
    background-image: url('https://wallpapercrafter.com/sizes/2560x1440/136245-Aperture-Laboratories-wall-texture-circle-digital-art-Portal-game-video-games.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    padding-top: 10vh;
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
