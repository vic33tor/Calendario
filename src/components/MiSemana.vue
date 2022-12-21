<template>
  <div class="grid grid-cols-7">
    <div
      v-for="(item, index) in days"
      :key="index"
      class="border-2 border-black p-4"
    >
      {{ item }}
    </div>
    <div
      v-for="(item, index) in days"
      :key="index"
      class="border-2 border-black p-4 h-screen"
    ></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      days: [
        "Lunes",
        "Martes",
        "Miercoles",
        "Jueves",
        "Viernes",
        "Sabado",
        "Domingo",
      ],
    };
  },
};
</script>

<style scoped></style>
