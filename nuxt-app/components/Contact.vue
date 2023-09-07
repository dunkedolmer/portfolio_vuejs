<script>
import ContactButton from './common/ContactButton.vue';

export default {
    components: {
        ContactButton
    },
    data() {
        return {
            info: {
                email: "frederik.rasmussen.privat@gmail.com" 
            }
        }
    }
};

</script>

<template>
    <div class="flex justify-center p-8">
        <!-- Left Column -->
        <div class="w-1/2 p-4 space-y-4">
            <h1 class="text-5xl font-bold">Contact</h1>
        <p>
            I can be contacted by email or through LinkedIn.
        </p>
        <ContactButton :email="info.email"/>
        </div>
        <!-- Right Column -->
        <div class="w-1/2 p-4">
            
        </div>

    </div>
</template>