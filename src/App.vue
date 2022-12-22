<template>
  <MiCabecera @cambiarVista="cambiarVista" />
  <div v-if="vista == 'day'">
    <MiDia />
  </div>
  <div v-else-if="vista == 'week'">
    <MiSemana />
  </div>
  <div v-else-if="vista == 'month'">
    <MiMes />
  </div>
</template>

<script>
import MiDia from "./components/MiDia.vue";
import MiSemana from "./components/MiSemana.vue";
import MiCabecera from "./components/MiCabecera.vue";
import MiMes from "./components/MiMes.vue";
export default {
  data() {
    return {
      vista: "day",
    };
  },
  methods: {
    cambiarVista(data) {
      console.log(data);
      if (data == "Semana") {
        this.vista = "week";
      } else if (data == "Mes") {
        this.vista = "month";
      } else {
        this.vista = "day";
      }
    },
  },
  components: { MiDia, MiSemana, MiCabecera, MiMes },
};
</script>

<style scoped></style>
