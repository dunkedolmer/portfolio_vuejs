<template>
    <button
      class="contact-button border border-teal-400 rounded-lg text-teal-400 font-mono text-base h-16 mx-auto px-8 py-2 transition duration-300 ease-in-out"
      @click="handleClick"
    >
      {{ email }}
    </button>
  </template>
  
  <script>
  export default {
    props: {
      email: String
    },
    methods: {
      handleClick() {
        if (this.email)
        {
            const mailtoLink = `mailto:${this.email}`;
            window.location.href = mailtoLink;
        }
        else
        {
            console.error("No email address provided")
        }
      }
    }
  };
  </script>
  