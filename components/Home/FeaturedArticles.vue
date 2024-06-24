<template>
  <div>
    <h2 class="uppercase text-sm font-semibold text-gray-400 mb-6">実務経験</h2>
    <ul class="space-y-16">
      <li v-for="(article, id) in articles" :key="id">
        <AppArticleCard :article="article" />
      </li>
    </ul>
  </div>
</template>

<script lang="ts" setup>
const { data: articles } = await useAsyncData("all-articles", () =>
  queryContent("/articles").sort({ id: -1 }).find()
);
</script>
