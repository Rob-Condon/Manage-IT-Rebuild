<template>
  <div class="flex justify-between content-between ph6 pv2" style="align-items: center" >
    <img :src='require("@/assets/ClientLogos/WindowTreatments.jpg")' class="no-flex"  alt="widnow treatments logo">
    <img :src='require("@/assets/ClientLogos/WildBerries.jpg")' class="no-flex" alt="wild berries logo">
    <img :src='require("@/assets/ClientLogos/ShantyTown.jpg")' class="no-flex" alt="shanty town logo">
    <img :src='require("@/assets/ClientLogos/FoxAndAssociates.jpg")' class="no-flex" alt="fox and associates logo">
    <img :src='require("@/assets/ClientLogos/KannangaraThomson.jpg")' class="no-flex" alt="Kannangara Thomson logo">
    <img :src='require("@/assets/ClientLogos/FurnitureSolutionsLogo.png")' class="no-flex" alt="Furniture Solutions Logo">
  </div>
</template>

<script>
export default {
  name: "BusinessStrip"
}
</script>

<style scoped>
.no-flex {
  flex: initial;
}
</style>