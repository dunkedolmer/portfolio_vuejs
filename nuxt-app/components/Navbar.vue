<script setup>
const route = useRoute();

const navigation = [
    { name: 'About', href: '#about', current: route.name == 'about' },
    { name: 'Work', href: '#work', current: route.name == 'work' },
    { name: 'Contact', href: '#contact', current: route.name == 'contact' },
]

</script>

<template>
    <nav class="fixed top-0 w-full p-4">
      <div class="flex items-center justify-between">
        <!-- Left div (Logo) -->
        <div class="flex items-center space-x-4">
          <router-link to="/" class="text-white">Logo</router-link> <!-- Insert logo here -->
        </div>
        <!-- Right div (Navigation) -->
        <div class="flex items-center space-x-4">
          <ul class="flex space-x-4">
            <li v-for="item in navigation" :key="item.name">
              <a :to="item.href" :class="{ 'hover:text-highlight': !item.current }" class="hover:text-highlight">
                {{ item.name }}
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </template>