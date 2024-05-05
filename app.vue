<template>
  <Header/>
  <v-divider :thickness="2" color="success"></v-divider>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script>
import Header from './components/layout/Header.vue'

export default {
  components: { Header },

}
</script>

<style>

</style>
