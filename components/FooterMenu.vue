<script setup lang="ts">
/**
 * @filename FooterMenu.vue
 * @author 김주현
 * @desc 푸터 메뉴
 */

let iconColor = '#424242';
let iconSize = '2rem';
let imgSrcs = [
    { label: '홈', src: '/images/footer-home.png' },
    { label: '오늘의 미션', src: '/images/footer-runner.png' },
    { label: '통계·보고', src: '/images/footer-chart.png' },
    { label: '포인트샵', src: '/images/footer-pointshop.png' },
    { label: '마이페이지', src: '/images/footer-profile.png' },
];

</script>


<template>
    <div class="py-2 px-3 border-t-2 flex justify-between">
        <div v-for="(item, i) in imgSrcs" :key="i" class="flex flex-col items-center">
            <NuxtImg :src="item.src" width="30px" />
            <p class="text-xs" style="color: #747474;">{{ item.label }}</p>
        </div>
    </div>
</template>