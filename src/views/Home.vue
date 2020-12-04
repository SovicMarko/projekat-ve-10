<template>
  <div class="home container">
    <div class="row">
      <div class="col col-xs-12 col-sm-6 col-md-4 col-lg-3"
           v-for="product in products" v-bind:key="product.id">
        <product-card v-bind:product="product"></product-card>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import ProductCard from '@/components/ProductCard.vue'

export default {
  name: 'Home',
  props: {
    products: Array
  },
  components: {
    ProductCard
  },
  data : function() {
    return {
      br1 : 20
    }
  }
}
</script>
