<script setup lang="ts">
import HeaderView from '~/components/HeaderView.vue';
import FooterMenu from '~/components/FooterMenu.vue';
</script>

<template>
  <!-- 헤더 -->
  <div class="h-screen flex flex-col">
    <HeaderView />

    <!-- 컨텐츠 영역 -->
    <div class="flex-grow p-5">
      <NuxtPage />
    </div>

    <!-- 푸터 메뉴 -->
    <FooterMenu />
  </div>

</template>
