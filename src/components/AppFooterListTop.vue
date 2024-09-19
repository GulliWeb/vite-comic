<script>
export default {
  data() {
    return {
        // creao array di oggetti per popolare le list
        menuItems: [
            {
              title: 'DC Comics',
              items: ['Characters', 'Comics', 'Movies', 'Games', 'Videos', 'News', 'Shop']
            },
            {
              title: 'DC',
              items: ['About Us', 'Privacy Policy', 'Ad Choices', 'Advertising', 'Jobs', 'FAQ', 'Investor Relations', 'Shop DC', 'DC Universe Infinite', 'DC Kids', 'DC Shop Locator', 'DC Power Visa']
            },
            {
              title: 'Sites',
              items: ['MAD Magazine', 'DC Daily', 'DC Universe']
            },
            {
              title: 'Shop',
              items: ['Shop DC', 'New 52']
            }
          ]
    }
  }
}
</script>

<template> 
  <div class="footer-top-wrapper">
    <ul class="d-flex">
      <li class="mt-5" v-for="(menu, index) in menuItems" :key="index">
        <strong class="li-title">{{ menu.title }}</strong>
        <ul>
          <li v-for="(item, i) in menu.items" :key="i">
            {{ item }}
          </li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
ul{
  padding-left: 0;
  margin-right: 50px;
  }

ul li{
    color: gray;
    list-style-type: none;
    padding-left: 0;
}

ul:first-child{
  margin-left: 300px
}

ul li:hover{
  color: white;
  cursor: pointer;
}

ul li:active{
  color: lightgray;
}

.li-title{
  color: white;
  font-weight: bold;
  font-size: larger;
}
</style>