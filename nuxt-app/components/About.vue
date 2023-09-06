<script>
export default {
  data() {
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
      ] 
      
    };
  }
};
</script>

<template>
    <div class="flex justify-center p-8">
        <!-- Left Column -->
        <div class="w-1/2 p-4 space-y-4">
            <h1 class="text-5xl">About Me</h1>
            <p>
                I'm a full-stack software developer based in Aalborg, Denmark. 
                I graduated my B.Sc in Software at Aalborg Universty in 2022 and will be finishing my M.Sc in Software in the summer 2024.
            </p>
            <p>
                I enjoy staying up to date with latest technologies and libraries as part of both my studies an spare time, but I am comfortable with:
                <ul class="list-disc pl-10 pt-2 space-y-2">
                    <li v-for="(item, index) in items" :key="index">{{ item }}</li>
                </ul>
            </p>
        </div>
        <!-- Right Column -->
        <div class="w-1/2 p-4">
            <img src="../assets/images/about-picture.jpg" class="rounded-full" alt="Picture"/>
        </div>

    </div>
</template>