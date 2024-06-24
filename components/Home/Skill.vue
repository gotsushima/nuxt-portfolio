<template>
  <div>
    <h2 class="uppercase text-sm font-semibold text-gray-400 mb-4">スキル</h2>
    <div class="space-y-5">
      <NuxtLink
        v-for="link in links"
        :key="link.icon"
        target="_blank"
        external
        class="flex items-end gap-4 group"
      >
        <span class="text-s">
          {{ link.name }}
        </span>
        <div
          class="flex-1 border-b border-dashed border-gray-300 dark:border-gray-800 group-hover:border-gray-700"
        ></div>
        <Icon :name="link.icon" class="w-6 h-6"></Icon>
      </NuxtLink>
    </div>
  </div>
</template>

<script lang="ts" setup>
const links = [
  {
    name: "JavaScript",
    icon: "mdi:language-javascript",
  },
  {
    name: "Vue",
    icon: "mdi:vuejs",
  },
  {
    name: "Nuxt",
    icon: "mdi:nuxt",
  },
  {
    name: "JQuery",
    icon: "mdi:jquery",
  },
  {
    name: "CSS",
    icon: "mdi:language-css3",
  },
  {
    name: "HTML",
    icon: "mdi:language-html5",
  },
  {
    name: "WordPress",
    icon: "mdi:wordpress",
  },
  {
    name: "Shopify",
    icon: "mdi:shopify",
  },
];
</script>
