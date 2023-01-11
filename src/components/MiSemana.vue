<template>
  <div class="grid grid-cols-7">
    <div
      v-for="(item, index) in days"
      :key="index"
      class="border-x border-y border-black p-4"
    >
      {{ item }}
    </div>
    <div
      v-for="(item, index) in days"
      :key="index"
      class="border-x border-black p-4"
    >
      <div
        v-for="(item, index) in 24"
        :key="index"
        class="border-b border-black p-4"
      >
        {{ item - 1 }}:00
      </div>
    </div>
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
