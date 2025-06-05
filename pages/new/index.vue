<script setup lang="ts">
const weight = ref<string>("");
const waist = ref<string>("");
const hips = ref<string>("");
const chest = ref<string>("");
</script>

<template>
  <div class="container p-4 bg-gray-100 min-h-dvh">
    <h2 class="text-5xl font-bold mb-7">Новый замер</h2>
    <div>
      <form>
        <h3 class="text-3xl mb-4">Добавление данных</h3>
        <InputNumber v-model="weight" placeholder="Вес (кг)" />
        <InputNumber v-model="waist" placeholder="Талия (см)" />
        <InputNumber v-model="chest" placeholder="Грудь (см)" />
        <InputNumber v-model="hips" placeholder="Бедра (см)" />
        <button
          type="submit"
          class="bg-green-800 active:bg-green-700 text-white text-2xl text-center rounded-md py-4 w-full"
        >
          Сохранить
        </button>
      </form>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
