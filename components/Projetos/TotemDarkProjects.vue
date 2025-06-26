<template>
    <div class="flex items-center justify-center bg-[#000136] rounded-4xl w-2xl p-10">
        <div class="">
            <h2 class="text-orange-500 text-2xl font-extrabold mb-4 uppercase">{{ titulo }}</h2>
            <ol class="list-decimal pl-5 text-justify text-white leading-relaxed mb-4">
                <li v-for="(item, index) in descricao" :key="index">
                {{ item }}
                </li>
            </ol>
            <div class="text-sm text-white mb-4">
                <span>Disponível em: <em>{{ link || '*link site da atlética*' }}</em></span>
            </div>
            <div class="w-full flex justify-center">
                <button class="flex bg-orange-500 hover:bg-orange-600 text-white font-bold py-2 px-6 rounded-full">
                    Saiba mais
                </button>
            </div>
        </div>
        </div>
    <div class="rounded-xl overflow-hidden mt-4">
        <img :src="imagem" :alt="titulo" class="w-full object-cover" />
    </div>
</template>

<script setup>
defineProps({
    titulo: String,
    descricao: Array,
    link:{
        type: String,
        default: '',
    },
    imagem: String
})
</script>