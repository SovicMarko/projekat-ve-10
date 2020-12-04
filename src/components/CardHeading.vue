<template>
   <div class="panel-heading" v-bind:style="`background-color: ${boja}`">
        <router-link v-bind:to="'/product/' + id">
            <h4>{{naziv}}</h4>
        </router-link>
   </div>
</template>

<script>
export default {
    name: "CardHeading",
    props: {
        id : Number,
        naziv : String,
        tip : String
    },
    computed: {
        boja: function() {
            if (this.tip == "graficka kartica") {
                return "#6d8985";
            } else if (this.tip == "procesor") {
                return "#5b5b68";
            } else if (this.tip == "monitor") {
                return "#8f6666"
            } else {
                return "white"
            }
        }
    }
}
</script>

<style scoped>
    a {
        color: white;
    }

</style>