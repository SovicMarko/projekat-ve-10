<template>
    <div>
        <h1 class="page-header">{{product.naziv}}</h1>
        <img v-bind:src="product.fotografija" alt="">
        <h3>{{product.cena}} RSD</h3>
    </div>
</template>

<script>
export default {
    name: "SingleProduct",
    props: {
        products: Array
    },
    computed: {
        product: function() {
            for (let i = 0; i < this.products.length; i++) {
               if (this.products[i].id == this.$route.params.id) {
                   return this.products[i];
               }
            }
            return false;
        }
    }
}
</script>

<style>

</style>