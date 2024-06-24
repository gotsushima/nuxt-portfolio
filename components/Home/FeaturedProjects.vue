<template>
  <div>
    <h2 class="uppercase text-sm font-semibold text-gray-400 mb-6">
      制作事例
    </h2>
    <div class="space-y-4">
      <AppProjectCard
        v-for="(project, id) in projects"
        :key="id"
        :project="project"
      />
    </div>
    <div class="flex items-center justify-center mt-6 text-sm">
      <UButton
        label="All Projects &rarr;"
        to="/projects"
        variant="link"
        color="gray"
      />
    </div>
  </div>
</template>

<script lang="ts" setup>
const { data: projects } = await useAsyncData("projects-home", () =>
  queryContent("/projects").limit(5).sort({ id: -1 }).find()
);
</script>
