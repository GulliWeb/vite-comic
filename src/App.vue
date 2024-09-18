<script>
// Importo i componenti nella mia app vue 
import AppFooter from "./components/AppFooter.vue";
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
export default {
  data() {
    return {
      
    }
  },
  // Registro i componenti in modo da poterli utilizzare nel template
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
</template>

<style lang="scss">
// @use "boostrap/scss/boostrap.scss" as *
@use "./styles/general.scss" as *
</style>
