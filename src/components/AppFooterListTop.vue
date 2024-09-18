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
              items: ['Shop DC', 'New 52', 'Digital Comics', 'Collectibles', 'Apparel', 'Funko', 'DC Comics Shop Locator']
            }
          ]
    }
  }
}
</script>

<template>
    
</template>

<style lang="scss" scoped>
ul li{
    color: white;
}
</style>