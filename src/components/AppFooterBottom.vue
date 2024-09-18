<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
    <button id="btn-sign" class="btn btn-primary">
        SIGN UP NOW!
    </button>
    <div class="right d-flex align-items-center">
        <p class="me-4 mb-0">FOLLOW US</p>
        <div class="social-icons">
            <button>
                <i class="fab fa-facebook-f"></i>
            </button>
            <button class="fab fa-twitter"></button>
            <button class="fab fa-youtube"></button>
            <button class="fab fa-pinterest-p"></button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#btn-sign{
    padding: 10px 15px;
    margin-left: 100px;
    background-color: transparent;
}

#btn-sign:hover{
    cursor: pointer;
    border: 2px solid rgb(56, 128, 241);
}

#btn-sign:active{
    color: lightgray;
    font-weight: normal;
}

.right{
    margin-right: 100px;
}

.right p{
    color: rgb(56, 128, 241);
    font-weight: bold;
    font-size: 18px;
}

.social-icons button{
    margin-right: 20px;
    height: 40px;
    width: 40px;
    text-align: center;
    background-color: rgb(121, 121, 121);
    color: rgb(48, 48, 48);
    border-radius: 50%;
}

.social-icons button:hover{
    color: lightgray;
    cursor: pointer;
}

.social-icons button:active{
    color: rgb(48, 48, 48);
}
</style>