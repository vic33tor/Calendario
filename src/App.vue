<template>
  <MiCabecera />
  <div>
    <MiDia />
  </div>
  <div>
    <MiSemana />
  </div>
  <div>
    <MiMes />
  </div>
</template>

<script>
import MiDia from "./components/MiDia.vue";
import MiSemana from "./components/MiSemana.vue";
import MiCabecera from "./components/MiCabecera.vue";
import MiMes from "./components/MiMes.vue";
export default {
  components: { MiDia, MiSemana, MiCabecera, MiMes },
};
</script>

<style scoped></style>
