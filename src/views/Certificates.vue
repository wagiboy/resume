<template>
  <div class="text-center">
    <v-carousel
      cycle
      show-arrows-on-hover
      height="100%"   
    >
      <v-carousel-item 
        v-for="(src, i) in slides" 
        :key="i"
        :src="src" 
       >
      </v-carousel-item>
    </v-carousel>

    <v-btn x-large color="primary" class="text-capitalize mt-5" to="/">
      close
      <v-icon>mdi-close</v-icon>
    </v-btn>
    
  </div>
</template>

<script>
export default {
  data: () => ({ 
    slides: [
      require('@/assets/udemy-cryptography-certificate.jpg'),
      require('@/assets/udemy-blockchain-certificate.jpg'),
      require('@/assets/udemy-solidity-certificate.jpg')
    ]
  }),
}
</script>