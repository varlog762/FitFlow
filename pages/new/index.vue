<script setup lang="ts">
const val = ref<string>("");

watch(val, () => {
  console.log(val.value);
});
</script>

<template>
  <div class="container p-4 bg-gray-100 min-h-dvh">
    <h2 class="text-5xl font-bold mb-7">Новый замер</h2>
    <div>
      <form>
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
