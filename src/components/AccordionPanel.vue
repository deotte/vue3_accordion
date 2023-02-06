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
  <div class="panel container mb-4 border-2 rounded-lg shadow-sm">
    <button
      @click.prevent="togglePanel"
      class="p-4 w-full border-b-2 font-semibold flex flex-row items-center justify-between">
      {{ title }}
      <span
        class="material-icons"
        v-if="showPanel">
        expand_more
      </span>
      <span
        class="material-icons"
        v-else>
        chevron_right
      </span>
    </button>
    <div
      class="content p-4"
      v-if="showPanel">
      <slot></slot>
    </div>
  </div>
</template>