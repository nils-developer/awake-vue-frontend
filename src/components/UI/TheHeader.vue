<template>
    <div class="header-div">
        <h1 class="header-h1">Awake</h1>
        <the-navbar></the-navbar>
    </div>
</template>

<script>

import TheNavbar from './TheNavbar.vue'

export default {
    components: {
        TheNavbar
    } 
}
</script>

<style scoped>
.header-h1 {
    font-size: 4.5rem;
    margin-left: 5rem;
}

.header-div {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>