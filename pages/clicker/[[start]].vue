<!-- src/pages/clicker/[[start]].vue -->
<script setup lang="ts">
import { ref, computed } from 'vue'
import { useRoute } from 'vue-router'

// 1) URL 파라미터 읽기
const route = useRoute()
const initial = computed(() => {
  // params.start 가 string | undefined
  const raw = route.params.start?.toString() ?? '0';
  const n = Number(raw);
  return isNaN(n) ? 0 : n;
})

// 2) 클릭 카운터 로직
const count = ref(initial.value)
function increment() {
  count.value++
}
</script>

<template>
  <div class="p-4">
    <h2 class="mb-2">
      시작값: {{ initial }} → 현재값: {{ count }}
    </h2>
    <button
      @click="increment"
      class="px-4 py-2 bg-blue-500 text-white border-2 rounded hover:cursor-pointer"
    >
      클릭!
    </button>
  </div>
</template>
