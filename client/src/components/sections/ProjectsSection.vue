<template>
  <div class="w-screen bg-stone-300 py-8 px-8 text-stone-800 text-justify section-index lg:pt-4">
    <div class="project-container container mx-auto">
      <h2 class="section-title">Projects</h2>
      <p>
        Here's a list of some of my related projects. Some where made as a
        freelance developer, and some as an individual contributor on a company.
      </p>
      <div class="project-grid container mx-auto">
        <div
          v-for="project of projects"
          :key="project.name"
          class="project-card bg-stone-700 text-stone-200 p-4 self-center min-h-[280px]"
        >
          <h2 class="text-center text-2xl mb-4">{{ project.name }}</h2>
          <p v-html="project.description" class="text-justify"></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const projects = [
  {
    name: "Kibun",
    description:
      "One page made for an award winning peruvian-japanese fusion restaurant. Worked as a freelancer as part of government sponsored digital marketing campaign. Made with BulmaCSS and vanilla Javascript.",
  },
  {
    name: "FROGAAS (Frogs as a Service)",
    description: "Frogs As A Service is an API REST that server random images of frogs. Inspired by Kevin Balicot's <a href='https://cataas.com/#/' class='text-orange-600'>CATAAS</a>. Made with Django and Django Rest Framework.",
  },
  {
    name: "Web Component Library",
    description:
      "Framework agnostic web component library. Made with Typescript and StencilJS.",
  },
  {
    name: "Integration with Keycloak",
    description:
      "Lead a team effort into integrating one of our Angular microfrontends with Keycloak. Made with Typescript.",
  },
  {
    name: "Website for a fintech startup",
    description:
      "Fully functional website for a fintech startup. Designed responsively to adapt to screens as small as 320px wide to full 4k resolution. Made with NuxtJS and TailwindCSS.",
  },

  {
    name: "Data dashboard for a law firm",
    description:
      "Refactored a legacy dashboard for a Django application into a modern, fast and responsive one. Made with Vue and ChartJS.",
  },
]
</script>

<style>
.project-container {
  @apply flex flex-col justify-between;
  gap: 2.5rem;
}

.project-grid {
  @apply grid justify-items-center justify-center;
  grid-template-columns: repeat(auto-fit, minmax(250px, 320px));
  row-gap: 1.75rem;
  column-gap: 2.25rem;
}
</style>
