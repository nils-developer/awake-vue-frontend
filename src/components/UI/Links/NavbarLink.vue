<template>
    <a href="#">
        <div class="nav-div">
            <h2>{{ label }}</h2>
        </div>
    </a>
</template>

<script>
export default {
    props: {
        label: {
            type: String,
            required: true,
        },
        link: {
            type: String,
            required: true,
        }
    }
}
</script>

<style scoped>

.nav-div {
    border: 2px solid white;
    border-radius: 5%;
    border-image-slice: 1;
    border-image-source: linear-gradient(to left, #111217 0%, #8c1aff);
    background-color: #111217;

    padding: .35rem .75rem;

    box-shadow: .5rem .35rem 0.2rem #21242c;
    transition: ease-in-out .2s;
}

.nav-div:hover {
    border-image-slice: 1;
    border-image-source: linear-gradient(to left, #8c1aff, #111217);
    transform: translateY(-.15rem);
    animation: moveBorder 3500ms infinite alternate linear;
}

h2 {
    margin: 0 auto;
}

@media(max-width: 1200px) {
    .nav-div {
        box-shadow: none;
    }
}
</style>