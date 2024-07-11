<script setup lang="ts">
import { useCounterStore } from "../store/counter";

const counterStore = useCounterStore();
</script>

<template>
  <div class="tw-grid tw-justify-center">
    <h1 class="tw-text-xl">Home {{ counterStore.count }}</h1>
    <q-btn color="primary" @Click="counterStore.increment" label="Primary" />
  </div>
</template>
