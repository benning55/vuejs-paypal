<template>
  <div class="about">
    <h1>Benning</h1>
    <div v-if="!paidFor">
      <h1>Buy this Lamp - ${{ product.price }} OBO</h1>

      <p>{{ product.description }}</p>

      <img width="400" src="https://images-na.ssl-images-amazon.com/images/I/61%2BhXJs1f3L._SL1500_.jpg" alt="">
    </div>

    <div v-if="paidFor">
      <h1>Noice, you bought a beautiful lamp!</h1>

      <img src="https://media1.giphy.com/media/BIzedshLe7maQ/giphy.gif?cid=790b7611074e68691af4481ec7f5d49148da475042fecefd&rid=giphy.gif" alt="">
      <div ref="paypal"></div>
    </div>
    
  </div>
</template>
