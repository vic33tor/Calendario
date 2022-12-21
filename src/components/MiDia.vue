<template>
  <div
    v-for="(item, index) in 24"
    :key="index"
    class="border-2 border-black p-4"
  >
    {{ item - 1 }}:00 - {{ item }}:00
  </div>
</template>

<script>
export default {};
</script>

<style scoped></style>
