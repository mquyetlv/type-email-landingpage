<template>
  <div class="card" :class="{ active: isActive }">
    <img class="rounded-[20px]" :src="props.card.image" alt="" />
    <div class="px-4 py-2">
      <h3 class="mt-3 mb-1 text-[18px] font-[600] text-[var(--primary-color)]">
        {{ props.card.title }}
      </h3>
      <p class="text-[20px] font-[600]">{{ props.card.descript }}</p>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";
const props = defineProps({
  card: {
    type: Object,
    required: true,
  },
  isActive: {
    type: Boolean,
    defalut: false,
  },
});
</script>

<style scoped>
.active {
  background: white;
}

.card {
  border-radius: 20px;
}
</style>
