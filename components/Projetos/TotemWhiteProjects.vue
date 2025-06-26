    <template>
        <div class="bg-[#D9D9D9] text-white p-6 rounded-xl shadow-lg max-w-2xl mx-auto">
            <div class="rounded-xl overflow-hidden mb-4">
                <img :src="imagem" :alt="titulo" class="w-full object-cover" />
            </div>
            
            <h2 class="text-orange-500 text-2xl font-extrabold mb-4 uppercase">{{ titulo }}</h2>
            
            <ol class="list-decimal pl-5 text-justify text-[#1F2171] leading-relaxed mb-4">
                <li v-for="(item, index) in descricao" :key="index">
                {{ item }}
                </li>
            </ol>
        
            <div class="text-sm text-[#1F2171] mb-4">
                <span>Disponível em: <em>{{ link || '*link site da atlética*' }}</em></span>
            </div>
            <div class="w-full flex justify-center">
                <button class="flex bg-orange-500 hover:bg-orange-600 text-white font-bold py-2 px-6 rounded-full">
                    Saiba mais
                </button>
            </div>
        </div>
    </template>
    
    <script setup>
    defineProps({
        titulo: String,
        imagem: String,
        descricao: Array,
        link: {
            type: String,
            default: ''
        }
    })
    </script>
    