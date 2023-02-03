<script setup>
  import AccordionPanel from './AccordionPanel.vue';
  import Contact from './Form/Contact.vue';
  import Shipping from './Form/Shipping.vue';
</script>

<template>
  <div class="accordion container mx-auto p-4">
    <AccordionPanel title="Contact Information">
      <Contact></Contact>
    </AccordionPanel>
    <AccordionPanel title="Shipping Information">
      <Shipping></Shipping>
    </AccordionPanel>
  </div>
</template>