<template>
    <the-header></the-header>
    <div id="about" class="about">
        <introducing></introducing>
        <projects></projects>
    </div>
    <div class="form-layout">
        <the-form></the-form>
    </div>
</template>

<script>
import TheHeader from './components/UI/TheHeader.vue';
import Introducing from './components/Introducing.vue';
import Projects from './components/Projects.vue';
import TheForm from './components/TheForm.vue'

export default {
  name: 'App',
  components: {
      TheHeader,
      Introducing,
      Projects,
      TheForm,
  }
}
</script>

<style>
.app {
    /*font-family: Avenir, Helvetica, Arial, sans-serif;*/
    font-family: Roboto, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: white;
    margin-top: 60px;
    width: 80vw;
    margin: 0 auto;
}

a {
    text-decoration: none;
    color: white;
}

.about {
    display: flex;
    justify-content: space-evenly;

    margin: 1rem 0;
}

.form-layout {
    display: flex;
    justify-content: center;
}
</style>
