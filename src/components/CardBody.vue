<template>
   <div class="panel-body">
        <img v-bind:src="fotografija" 
             v-bind:alt="naziv">
        <div v-if="popust"
             class="popust">
             -{{popust}}%
             <div class="triangle-down"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: "CardBody",
    props: {
        fotografija : String,
        naziv: String,
        popust: Number
    }
}
</script>

<style scoped>
    .panel-body {
        height: 280px;
        line-height: 280px;
        position: relative;
    }
    .popust {
        position: absolute;
        right: 15px;
        top: 0px;
        background-color: khaki;
        width: 70px;
        height: 60px;
        line-height: 60px;
        text-align: center;
        font-size: 20px;
    }
    .triangle-down {
      width: 0;
      height: 0;
      border-left: 35px solid transparent;
      border-right: 35px solid transparent;
      border-top: 20px solid khaki;
    }
  
    img {
        width: 100%;
    }
</style>