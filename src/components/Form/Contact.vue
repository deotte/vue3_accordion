<script setup>
  import { reactive } from 'vue';

  const state = reactive({
    fullName: '',
    email: '',
    phoneNumber: ''
  });
</script>

<template>
  <div class="input">
    <label for="fullName">Full Name</label>
    <input
      type="text"
      id="fullName"
      name="fullName"
    />
  </div>
  <div class="input">
    <label for="email">Email</label>
    <input
      type="text"
      id="email"
      name="email"
    />
  </div>
  <div class="input">
    <label for="phoneNumber">Phone Number</label>
    <input
      type="text"
      id="phoneNumber"
      name="phoneNumber"
    />
  </div>
</template>