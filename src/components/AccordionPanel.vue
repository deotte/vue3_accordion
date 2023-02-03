<script setup>
  import { ref } from 'vue';

  const props = defineProps({
    title: { type: String, required: true }
  });

  const showPanel = ref(false);

  const togglePanel = (event) => {
    showPanel.value = !showPanel.value;
  }
</script>

<template>
  <div class="panel container mb-2 border-2 rounded-lg shadow-sm">
    <button
      @click.prevent="togglePanel"
      class="p-4 w-full text-left border-b-2 font-semibold text-lg">
      {{ title }}
      <span class="bold">></span>
    </button>
    <div
      class="content p-4"
      v-if="showPanel">
      <slot></slot>
    </div>
  </div>
</template>