<script setup lang="ts">
const model = defineModel();
</script>

<template>
  <div>
    <input
      v-model="model"
      type="number"
      placeholder="Вес (кг)"
      class="text-2xl py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-4"
    />
  </div>
</template>

<style lang="scss" scoped></style>
