<template>
  <NuxtLink
    class="flex items-end gap-4 group p-2 -m-2 rounded-lg"
    :to="project.url"
    target="_blank"
    external
  >
    <div class="">
      <h3 class="text-s  group-hover:text-primary-600 text-gray-700 dark:text-gray-200">
        {{ project.name }}
      </h3>
      <p class="text-gray-600 dark:text-gray-200 text-s font-bold">{{ project.description }}</p>
    </div>
    <div
      class="flex-1 border-b border-dashed border-gray-300 dark:border-gray-800 group-hover:border-gray-700"
    ></div>
  </NuxtLink>
</template>

<script setup>
defineProps({
  project: {
    type: Object,
    required: true,
  },
});
</script>
