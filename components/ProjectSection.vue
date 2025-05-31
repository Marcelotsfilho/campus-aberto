<template>
    <section class="my-12 text-center">
        <h2 class="text-start text-xl md:text-2xl font-bold text-orange-600 mb-20">{{ title }}</h2>
        <div class="flex flex-wrap justify-center gap-30">
            <MemberCard
            v-for="member in members"
            :key="member.name"
            :name="member.name"
            :role="member.role"
            :image="member.image"
            :linkedin="member.linkedin"
            :github="member.github"
            />
        </div>
        <button class="
                    mt-20 
                    bg-orange-500 
                    hover:bg-orange-600 
                    transition 
                    text-white 
                    font-semibold 
                    py-2 
                    px-6 
                    rounded-full 
                    shadow-md
                ">Saiba mais
        </button>
        <div class="mt-10 h-1 bg-[#0b0b35]"></div>
    </section>
  </template>
  
<script setup>
    import MemberCard from './MemberCard.vue';
    
    defineProps({
        title: String,
        members: Array,
    });
</script>
  