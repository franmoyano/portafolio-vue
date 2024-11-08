<script setup>
import Education from './components/Education.vue';
import NavBar from './components/NavBar.vue';
import Presentation from './components/Presentation.vue';
</script>

<template>
  <div class="container">
    <header>
      <NavBar />
    </header>

    <main>
      <Presentation />
      <Education />
    </main>
  </div>
</template>

<style lang="css">
.container {
  width: 100%;
  margin: 0px;
}
</style>