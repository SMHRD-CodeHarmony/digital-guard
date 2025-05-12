<script setup lang="ts">
/**
 * @file ContentCard.vue
 * @author 김주현
 * @desc 동적 색상의 카드형태 div 컨테이너
 */

defineProps<{
  background?: string;
  color?: string;
  weight?: string;
}>();
</script>

<template>
  <div :class="['rounded p-3 border', background, color, weight]">
    <slot></slot>
  </div>
</template>
