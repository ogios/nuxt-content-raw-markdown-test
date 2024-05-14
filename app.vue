<script setup lang="ts">
const { data } = await useAsyncData("test", () =>
  queryContent("/test").findOne(),
);
console.log(data);
</script>

<template>
  <div>{{ data }}</div>
</template>
