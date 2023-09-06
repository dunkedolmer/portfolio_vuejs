<script>
export default {
  data() {
    return {
      name: "I'm Frederik Rasmussen",
      smallIntro: "I'm a software engineering student currently specializing in Machine Intelligence"
    };
  },
  methods: {
    
  }
};
</script>

<template>
    <div class=" flex flex-col text-center p-20 space-y-4">
        <h5 class="text-highlight text-base font-extralight ">Hello</h5>
        <div class="">
            <span class="text-5xl" v-for="(char, index) in name" :key="index">{{ char }}</span>
        </div>
        <div class="text-lg">
            {{ smallIntro }}
        </div>
    </div>
</template>