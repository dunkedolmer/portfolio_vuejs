<script>
import Description from './common/Description.vue';

export default {
  data()
  {
    return {
      items:
        [
          ".NET (C#)",
          "Python",
          "JavaScript (ES6, Node.js, ReactJS)",
          "HTML/CSS",
          "TypeScript (Vue.js)",
          "Docker",
          "Kubernetes",
          "SQL (PostgreSQL, MySQL)"
        ],
      descriptions:
      {
        mainDescription: "I'm a full-stack software developer based in Aalborg, Denmark. I graduated my B.Sc in Software at Aalborg Universty in 2022 and will be finishing my M.Sc in Software in the summer 2024.",
        subDescription: "I enjoy staying up to date with latest technologies and libraries as part of both my studies and spare time, but I am comfortable with:"
      }

    };
  }
};
</script>

<template>
  <div class="flex justify-center p-8">
    <!-- Left Column -->
    <div class="w-1/2 p-4 space-y-4">
      <h1 class="text-5xl font-bold">About Me</h1>
      <p>{{ descriptions.mainDescription }}</p>
      <p>
        {{ descriptions.subDescription }}
      <ul class="list-disc pl-10 pt-2 space-y-2">
        <li v-for="(item, index) in items" :key="index">{{ item }}</li>
      </ul>
      </p>
    </div>
    <!-- Right Column -->
    <div class="flex items-center justify-center w-1/2 p-4">
      <img src="../assets/images/about-picture.jpg" class="rounded-full object-cover w-80 h-80" alt="Photo" />
    </div>

  </div>
</template>