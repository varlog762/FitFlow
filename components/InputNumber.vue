<script setup lang="ts">
const model = defineModel<string>();
const { placeholder } = defineProps<{
  placeholder: string;
}>();
</script>

<template>
  <div>
    <input
      v-model="model"
      type="number"
      :placeholder="placeholder"
      class="text-2xl py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-4"
    />
  </div>
</template>

<style lang="scss" scoped></style>
