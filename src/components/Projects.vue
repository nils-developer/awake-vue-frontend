<template>
    <div class="projects">
        <div class="projects-div">
            <a href="https://github.com/nils-developer/nils-developer" target="_blank">

                <div class="projects-div-content">
                    <h3>Github Profile</h3>
                    <p class="projects-p">Das ist mein Github Profil. In diesem Profil findest du Projekte an denen ich gerade arbeite und 
                        Projekte die ich bereits abgeschlossen habe.
                    </p>
                </div>
            </a>
        </div>
        <div class="projects-div">
            <a href="https://github.com/nils-developer/awake-vue-frontend" target="_blank">
                <div class="projects-div-content">
                    <h3>Project: Awake</h3>
                    <p class="projects-p">
                        Ein simples Frontend Projekt mit Vue.js
                    </p>
                </div>
            </a>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.projects {
    display: flex; 
    flex-direction: column;

    max-width: 45%;
}

.projects-div {
    display: flex;
    
    align-items: center;

    text-align: left;

    margin-bottom: 1.5rem;

    height: 20vh;
    min-height: 10rem;

    background-color: #15171e;

    border-radius: .65rem;

    transition: ease-in-out .2s;
}

.projects-div:hover {
    transform: translateX(.25rem);

    box-shadow: .1rem .1rem .35rem black;
}

.projects-div-content {
    padding: 1rem 2rem;
}

.projects-p {
    color: #898c91;
}
</style>