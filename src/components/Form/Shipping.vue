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
    <label class="font-semibold" for="address">Address</label>
    <input
      class="block inner-shadow rounded border-2 w-full mt-2 p-1"
      type="text"
      id="address"
      name="address"
    />
  </div>
  <div class="input mt-4">
    <label class="font-semibold" for="city">City</label>
    <input
      class="block inner-shadow rounded border-2 w-full mt-2 p-1"
      type="text"
      id="city"
      name="city"
    />
  </div>
  <div class="input mt-4">
    <label class="font-semibold" for="state">State</label>
    <input
      class="block inner-shadow rounded border-2 w-1/2 mt-2 p-1"
      type="text"
      id="state"
      name="state"
    />
  </div>
</template>