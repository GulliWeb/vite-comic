<script>
export default {
  data() {
    return {
        // Creo array di oggetti per popolare la scrollBar
     scrollList: [
        {src: '@/assets/img/buy-comics-digital-comics.png', name: "DIGITAL COMICS"},
        {src: "./img/buy-comics-merchandise.png", name: "SC MERCHANDISE"},
        {src: "./img/buy-comics-subscriptions.png", name: "SUBSCRIPTION"},
        {src: "./img/buy-comics-shop-locator.png", name: "COMIC SHOP LOCATOR"},
        {src: "./img/buy-dc-power-visa.svg", name: "DC POWER VISA"}
     ] 
    }
  },
  methods:{
    getImageUrl(path){
        return new URL(path, import.meta.url).href;
    }
  }
}
</script>

<template>
    <ul class="d-flex justify-content-between">
        <li class="d-flex align-items-center me-5" v-for="item in scrollList">
            <img :src="item.src">
            <p id="item-name">
                {{ item.name }}
            </p>
        </li>
    </ul>
    
</template>

<style lang="scss" scoped>
ul{
    margin-bottom: 0;
}

ul li{
    list-style-type: none;
}

#item-name{
    margin-left: 20px;
}

ul li img{
    max-width: 70px;
}
</style>