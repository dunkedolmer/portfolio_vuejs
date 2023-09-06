<script setup>
const route = useRoute();

const navigation = [
    { name: 'About', href: '#about', current: route.name == 'about' },
    { name: 'Work', href: '#work', current: route.name == 'work' },
    { name: 'Contact', href: '#contact', current: route.name == 'contact' },
]

</script>

<template>
    <nav class="p-4">
        <div class="container flex justify-between items-center">
            <router-link to="/" class="text-white">Logo</router-link> <!-- Insert logo here -->
            <ul class="flex space-x-4">
                <li v-for="item in navigation" :key="item.name">
                    <a :to="item.href" :class="{ 'hover:text-highlight': !item.current }" class="hover:text-highlight">
                        {{ item.name }}
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<!-- Bar -->
<!-- 
        box-sizing: border-box;
    font-family: sans-serif;
    margin: 0;
    background-color: #0a192f;
    height: 70px;
    justify-content: space-around;
    padding-top: 10px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 3;
    align-items: center;
    display: flex;
 -->

<!-- Item -->
<!-- 
    box-sizing: border-box;
    font-family: sans-serif;
    margin: 0;
    color: #ccd6f6;
    transition: .3s;
 -->