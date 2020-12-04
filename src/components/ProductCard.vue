<template>
    <div class="panel panel-danger">
        <card-heading 
            v-bind:naziv="product.naziv" 
            v-bind:id="product.id"
            v-bind:tip="product.tip"/>
        <card-body 
            v-bind:fotografija="product.fotografija" 
            v-bind:naziv="product.naziv"
            v-bind:popust="product.popust"/>
        <div class="panel-footer">
            <h3>{{product.cena}} RSD</h3>
        </div>
       
    </div>
</template>

<script>
import CardHeading from "./CardHeading.vue"
import CardBody from "./CardBody.vue"

export default {
    name: "ProductCard",
    components: {
        CardHeading,
        CardBody
    },
    props: {
        product : Object
    }
}
</script>

<style scoped>
    .panel-heading {
        height: 80px;
    }
    
</style>