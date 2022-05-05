<template>
    <div class="intro-div">
        <div>
            <h2 class="intro-h2">
                    Interface Designer & 
                    <br>
                    Full-Stack Developer
            </h2>
        </div>
        <div class="intro-p-div">
            <p class="intro-p">
                Seit 2021 erschaffe ich zusammen mit meinen Kunden als freiberuflicher Interface Designer und Front-End Developer, 
                einfache, interaktive Lösungen für komplexe Probleme. Aktuell unterstütze ich als Senior Front-End Developer die Gothaer Systems GmbH 
                und beschäftige mich meistens mit UI/UX Design, Angular, NodeJS, Flutter und allem, was mit Front-End zu tun hat.
            </p>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.intro-div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    width: 45%;
    height: 60vh;

    background-color: #15171e;
    border-radius: .65rem;

    transition: ease-in-out .25s;
    transition-delay: 100ms;

    padding: 2.5rem 0;
}

.intro-div:hover {
    padding: 4rem 0;
}

.intro-h2 {
    font-size: 2.5rem;
}

.intro-p-div {
    width: 60%;
    text-align: left;
}

.intro-p {
    color: #898c91;
    line-height: 1.5rem;
}
</style>