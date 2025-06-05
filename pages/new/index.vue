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
        <input
          v-model="weight"
          type="number"
          placeholder="Вес (кг)"
          class="text-2xl py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-4"
        />
        <input
          v-model="waist"
          type="number"
          placeholder="Талия (см)"
          class="py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-4"
        />
        <input
          v-model="chest"
          type="number"
          placeholder="Грудь (см)"
          class="py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-4"
        />
        <input
          v-model="hips"
          type="number"
          placeholder="Бедра (см)"
          class="py-4 px-1 w-full rounded-md border-2 border-gray-400 mb-10"
        />
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
