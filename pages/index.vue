<script setup lang="ts"></script>

<template>
  <div class="container p-4 bg-gray-100 min-h-dvh">
    <h2 class="text-5xl font-bold mb-7">Сегодняшний прогресс</h2>
    <div class="grid gap-3 grid-cols-2 grid-rows-2 mb-3">
      <ProgressCard />
      <ProgressCard />
      <ProgressCard />
      <ProgressCard />
    </div>
    <div class="bg-white rounded-md p-4">
      <h3 class="progress-card-title text-2xl mb-2">Осталось до цели:</h3>
      <div class="progress-card-change text-xl text-green-800">
        -5 кг, -6 cm
      </div>
    </div>
    <div class="px-4 absolute bottom-20 left-0 w-full">
      <NuxtLink
        to="/new"
        class="flex items-center justify-center gap-1 bg-green-800 hover:bg-green-700 text-white text-2xl text-center rounded-md py-4"
      >
        <Icon name="uil:plus" style="color: white" />
        Добавить замер
      </NuxtLink>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
