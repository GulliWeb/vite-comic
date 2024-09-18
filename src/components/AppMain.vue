<script >
import MainScroll from './MainScroll.vue';
export default {
  data() {
    return {
    }
  },
  components:{
    MainScroll
  }
}
</script>

<template>
<main>
    <div class="content-top-wrapper d-flex align-items-center">
        <h1> --> CONTENT GOES HERE <--</h1>
    </div>
    <div class="content-bottom-wrapper d-flex align-items-center justify-content-between">
        <MainScroll/>
    </div>
</main>
</template>

<style scoped>
.content-top-wrapper{
    height: 150px;
    background-color: #000;
}

.content-top-wrapper > *, .content-bottom-wrapper > *{
    margin-left: 320px;
}

.content-bottom-wrapper{
    height: 150px;
    background-color: rgb(56, 128, 241);
    color: white;
}
</style>  