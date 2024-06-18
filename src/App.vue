<script setup lang="ts">
import { RouterView } from 'vue-router'
import NavBar from '@/shared/components/NavBar.vue'
import { routerLinks } from '@/router/list-routes'
</script>

<template>
  <main>
    <header>
      <NavBar title="PokemonApp" :links="routerLinks" />
    </header>

    <RouterView />
  </main>
</template>
<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}
main {
  height: 100vh;
  width: 100vw;
  padding: 25px;
}
</style>
