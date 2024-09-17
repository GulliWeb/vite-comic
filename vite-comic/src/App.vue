<script>
// Importo i componenti nella mia app vue 
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"

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

<style scoped>
</style>
