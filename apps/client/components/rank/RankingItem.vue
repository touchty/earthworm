<template>
  <div
    class="flex h-[40px] items-center justify-between border-b border-gray-200 text-sm dark:border-gray-600"
  >
    <RankRankingBadge
      class="w-16"
      :rank="rank"
    />
    <div class="flex-1 truncate text-center">{{ username || "匿名" }}</div>
    <div class="w-16 text-right">{{ count }} 课</div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  rank: Number,
  username: String,
  count: Number,
});
</script>
