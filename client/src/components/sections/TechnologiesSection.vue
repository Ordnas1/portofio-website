<template>
  <section class="bg-stone-800 w-screen gap-4 text-slate-100 section-index">
    <div class="container mx-auto p-8 flex flex-col justify-evenly gap-10">
      <h2 class="text-4xl font-inter text-center font-semibold">
        Technologies
      </h2>
      <p class="text-justify">
        These are some of the languages, frameworks, tools and technologies that
        I have worked with in the past.  I'm by no means limited to only these, as I strive to learn on the go
        and adapt to the existing conventions of my team.
      </p>
      <div class="flex justify-center items-center gap-8 flex-wrap">
        <TechBadge>
          <i class="fa-brands fa-angular text-4xl"></i>
          <p class="">Angular</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-react text-4xl"></i>
          <p class="">React</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-vuejs text-4xl"></i>
          <p class="">Vue</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-html5 text-4xl"></i>
          <p class="">HTML</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-css3-alt text-4xl"></i>
          <p class="">CSS</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-sass text-4xl"></i>
          <p class="">Sass</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-node-js text-4xl"></i>
          <p class="">NodeJS</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-python text-4xl"></i>
          <p class="">Python</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-golang text-4xl"></i>
          <p class="">Go</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-docker text-4xl"></i>
          <p class="">Docker</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-solid fa-database text-4xl"></i>
          <p class="">Postgres</p>
        </TechBadge>
        <TechBadge>
          <i class="fa-brands fa-git-alt text-4xl"></i>
          <p class="">Git</p>
        </TechBadge> 
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
import TechBadge from "../elements/TechBadge.vue";
</script>
