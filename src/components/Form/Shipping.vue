<script setup>
  import { reactive } from 'vue';

  const state = reactive({
    address: '',
    city: '',
    state: ''
  });
</script>

<template>
  <div class="input">
    <label for="address">Address</label>
    <input
      type="text"
      id="address"
      name="address"
    />
  </div>
  <div class="input">
    <label for="city">City</label>
    <input
      type="text"
      id="city"
      name="city"
    />
  </div>
  <div class="input">
    <label for="state">State</label>
    <input
      type="text"
      id="state"
      name="state"
    />
  </div>
</template>