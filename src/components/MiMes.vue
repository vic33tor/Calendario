<template>
  <div
    v-for="(item, index) in mes"
    :key="index"
    class="border-2 border-black p-4"
  >
    {{ item }}
  </div>
</template>

<script>
export default {};
</script>

<style scoped></style>
