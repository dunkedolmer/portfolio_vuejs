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
        <div class="relative">
            <span 
              class="text-5xl font-bold hover:transform hover:translate-y-2 hover:text-highlight cursor-pointer" 
              v-for="(char, index) in name" 
              :key="index">
              {{ char }}
            </span>
        </div>
        <div class="text-lg">
            {{ smallIntro }}
        </div>
    </div>
</template>
<!--     color: #ccd6f6;
    font-size: 55px;
    box-sizing: border-box;
    margin: 0;
    bottom: 0;
    font-family: Poppins,sans-serif;
    font-weight: 800;
    transition: .3s;
    position: relative; -->