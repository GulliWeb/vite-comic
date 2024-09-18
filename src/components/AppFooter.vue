<script>
import AppFooterListTop from './AppFooterListTop.vue'
import AppFooterBottom from './AppFooterBottom.vue'
export default {
  data() {
    return {
      
    }
  },
  components:{
    AppFooterListTop,
    AppFooterBottom
  }
}
</script>

<template>
  <footer>
    <AppFooterListTop/>

    <div class="footer-bottom d-flex align-items-center justify-content-between">
    <AppFooterBottom/>

    </div>
  </footer>
    
    

</template>

<style scoped>
footer{
  background-image: url(../img/footer-bg.jpg);
}

.footer-bottom{
  height: 144px;
  background-color: rgb(48, 48, 48);
}
</style>