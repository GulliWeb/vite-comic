<script>
export default {
  data() {
    return {
        // Creo array di oggetti per popolare la scrollBar
     scrollList: [
        {src: "src/img/buy-comics-digital-comics.png", name: "DIGITAL COMICS"},
        {src: "src/img/buy-comics-merchandise.png", name: "SC MERCHANDISE"},
        {src: "src/img/buy-comics-subscriptions.png", name: "SUBSCRIPTION"},
        {src: "src/img/buy-comics-shop-locator.png", name: "COMIC SHOP LOCATOR"},
        {src: "src/img/buy-dc-power-visa.svg", name: "DC POWER VISA"}
     ] 
    }
  },
  methods:{
    getImageUrl(path){
        return new URL(`../${path}`, import.meta.url).href;
    }
  }
}
</script>

<template>
    <ul class="d-flex justify-content-between">
        <li class="d-flex align-items-center me-5" v-for="item in scrollList">
            <img :src="item.src">
            <p id="item-name" >
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
    text-wrap: nowrap;
}

ul li:hover{
    color: lightgray;
    cursor: pointer;
}

ul li:active{
    color: white;
}

#item-name{
    margin-left: 20px;
    
}

ul li img{
    max-width: 50px;
}
</style>