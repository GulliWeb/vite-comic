<script >
import MainContent from './MainContent.vue';
import MainScroll from './MainScroll.vue';
export default {
  data() {
    return {
    }
  },
  components:{
    MainScroll,
    MainContent
  }
}
</script>

<template>
<main>
    <div class="content-top-wrapper">
      <figure>
        <img src="../img/jumbotron.jpg" alt="">
      </figure>
      <MainContent/>
    </div>
    <div class="content-bottom-wrapper d-flex align-items-center justify-content-between">
        <MainScroll/>
    </div>
</main>
</template>

<style scoped>
figure{
  width: 100%;
  height: fit-content;
  margin: 0;
}

img{
  width: 100%;
  max-height: 400px;
  object-fit: cover;
  object-position: top;
}
.content-top-wrapper{
  width: 100%;
    background-color: #000;
}

 .content-bottom-wrapper > *{
    margin-left: 320px;
}

.content-bottom-wrapper{
    height: 150px;
    background-color: rgb(56, 128, 241);
    color: white;
}
</style>  