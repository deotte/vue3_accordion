<script setup>
  import AccordionPanel from './AccordionPanel.vue';
  import Contact from './Form/Contact.vue';
import CustomerWarning from './Form/CustomerWarning.vue';
  import Shipping from './Form/Shipping.vue';
</script>

<template>
  <div class="accordion container mx-auto p-4">
    <div class="header flex flex-row items-center justify-between py-2 border-b-2 mb-4">
      <h2 class="text-2xl">Payment</h2>
      <h2 class="text-2xl">Order #98765</h2>
    </div>
    <form>
      <AccordionPanel
        aria-title="contact"
        title="Contact Information">
        <Contact></Contact>
      </AccordionPanel>
      <AccordionPanel
        aria-title="shipping"
        title="Shipping Information">
        <Shipping></Shipping>
      </AccordionPanel>
      <AccordionPanel
        aria-title="incidents"
        title="Tracking Incidents">
        <CustomerWarning></CustomerWarning>
      </AccordionPanel>
    </form>
  </div>
</template>