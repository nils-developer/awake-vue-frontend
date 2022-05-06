<template>
    <button class="form-button">{{ label }}</button>
</template>

<script>
export default {
    props: {
        label: {
            type: String,
            required: true,
        },
    },
}
</script>

<style scoped>
.form-button {
    border: 2px solid white;
    border-radius: 5%;
    border-image-slice: 1;
    border-image-source: linear-gradient(to left, #111217 0%, #8c1aff);

    width: 10rem;
    height: 2.5rem;
    font-size: 1.25rem;

    color: white;
    background-color: #21242c;

    transition: ease-in-out .2s;
}

.form-button:hover {
    cursor: pointer;
    border-image-slice: 1;
    border-image-source: linear-gradient(to left, #8c1aff, #111217);
    transform: translateY(-.15rem);
    animation: moveBorder 3500ms infinite alternate linear;
}

.form-button:active {
    transition: .1s ease-out;
    transform: translateY(.1rem);
}
</style>