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
    name: "Vue.js",
    icon: "mdi:vuejs",
  },
  {
    name: "jQuery",
    icon: "mdi:jquery",
  },
  {
    name: "php",
    icon: "mdi:language-php",
  },
  {
    name: "WordPress",
    icon: "mdi:wordpress",
  },
  {
    name: "Dart",
    icon: "mdi:google",
  },
  {
    name: "Flutter",
    icon: "mdi:cellphone",
  },
  {
    name: "CSS",
    icon: "mdi:language-css3",
  },
  {
    name: "SASS",
    icon: "mdi:sass",
  },
  {
    name: "HTML",
    icon: "mdi:language-html5",
  },
  {
    name: "Shopify",
    icon: "mdi:shopify",
  },
];
</script>
