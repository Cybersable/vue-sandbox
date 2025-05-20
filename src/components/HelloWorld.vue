<script setup lang="ts">

defineProps<{ msg: string }>()

</script>

<template>
  <h1 color="$ep-color-primary">
    {{ msg }}
  </h1>
</template>
