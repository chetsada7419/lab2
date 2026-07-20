<script setup lang="ts">
import type { Event } from '@/types'

defineProps<{
  event: Event
}>()
</script>

<template>
  <div class="category-card">
    <p>{{ event.category }}</p>
    <p>{{ event.organizer }}</p>
  </div>
</template>

<style scoped>
.category-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
  text-align: right;
}

.category-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}

.category-card p {
  margin: 0;
  font-size: 16px;
}
</style>