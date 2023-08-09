<template>
  <button @click="handeEmit">{{ props.text }}</button>
</template>

<script setup>
  import { defineProps, defineEmits } from 'vue';
  const emit = defineEmits(['clickButton']);

  const props = defineProps({
    text: {
      type: String,
      default: 'No text specify',
    }
  });

  function handeEmit() {
    emit('clickButton', 999);
  }
</script>