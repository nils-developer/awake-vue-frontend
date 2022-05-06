<template>
    <nav class="navbar">
        <navbar-link class="navbar-link" link="#" label="Home"></navbar-link>
        <navbar-link class="navbar-link" link="#about" label="About"></navbar-link>
        <navbar-link class="navbar-link" link="#" label="+"></navbar-link>
    </nav>
</template>

<script>
import NavbarLink from './Links/NavbarLink.vue'

export default {
    components: {
        NavbarLink,
    }    
}
</script>

<style scoped>
.navbar {
    display: flex;
    justify-content: space-evenly;
    width: 20vw;
}

@media(max-width: 1200px) {
    .navbar-link {
        margin: 0rem 1rem;
    }
}
</style>