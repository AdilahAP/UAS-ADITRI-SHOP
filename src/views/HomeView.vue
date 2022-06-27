<template>
  <div>
    <div class="app-page-title">
      <div class="page-title-wrapper">
        <div class="page-title-heading">
          <div class="page-title-icon">
            <i class="pe-7s-home icon-gradient bg-mean-fruit">
            </i>
          </div>
          <div>Beranda</div>
        </div>
      </div>
    </div>
  </div>
  
  <div class="home">
    <Navbar />
    <div class="container">
      <Hero />

      <div class="row mt-4">
        <div class="col">
          <h2>
            Best
            <strong>Merchandise</strong>
          </h2>
        </div>
        
      </div>

      <div class="row mb-4">
        <div class="col-md-4 mt-4" v-for="product in products" :key="product.id">
          <CardProduct :product="product"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardProduct from '@/components/CardProduct.vue'
import Hero from '@/components/Hero.vue'
import axios from 'axios';

export default {
  name: 'HomeView',
  components: {
    CardProduct,
    Hero,
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProducts(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3000/products")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log(error))
  },
}
</script>
