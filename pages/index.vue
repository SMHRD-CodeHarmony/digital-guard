<script setup lang="ts">
import ContentCard from '~/components/ContentCard.vue';
</script>

<template>
  <div class="flex flex-col gap-3">

    <ContentCard background="bg-amber-100" color="border-amber-400" weight="border-2">
      <p>카드 1</p>
    </ContentCard>

    <ContentCard background="bg-sky-100" color="border-sky-400" weight="border-2">
      <p>카드 2</p>
    </ContentCard>

    <ContentCard background="bg-purple-100" color="border-purple-400" weight="border-2">
      <p>카드 3</p>
    </ContentCard>
  </div>

</template>
