<script setup>
  const props = defineProps({
    title: { type: String, required: true }
  })
</script>

<template>
  <div class="panel">
    <button>{{ title }}</button>
    <div class="content">
      <slot></slot>
    </div>
  </div>
</template>