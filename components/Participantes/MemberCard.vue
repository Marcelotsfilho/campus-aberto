<template>
    <div class="bg-[#0b0b35] text-white rounded-2xl overflow-hidden shadow-lg w-64 flex flex-col items-center">
        <img :src="image" :alt="name" class="w-full h-72 object-cover border-b-4 border-orange-500" />
        <div class="p-4 text-center">
            <h3 class="text-lg font-semibold">{{ name }}</h3>
            <p class="text-sm mb-2">{{ role }}</p>
            <div class="flex justify-center gap-4 mt-2">
                <a v-if="lattes" :href="lattes" target="_blank" class="hover:text-orange-400 transition">
                    <img src="/assets/images/Lattes.png" />
                </a>
                <a v-if="linkedin" :href="linkedin" target="_blank" class="hover:text-orange-400 transition">
                    <img src="/assets/images/LinkedIn.png" />
                </a>
                <a v-if="github" :href="github" target="_blank" class="hover:text-orange-400 transition">
                    <img src="/assets/images/GitHub.png" />
                </a>
            </div>
        </div>
    </div>
</template>
  
<script setup>
    defineProps({
        name: String,
        role: String,
        image: String,
        lattes: String,
        linkedin: String,
        github: String,
    });
</script>
  