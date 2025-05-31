<script setup>
import BannerParticipantes from '@/components/BannerParticipantes.vue';
import ProjectSection from '@/components/ProjectSection.vue';

// Imagens (ajuste os caminhos conforme necessário)
import gabriela from '@/assets/images/gabriela.jpg';
// import runnerImg from '@/assets/images/OutraPessoa.jpeg';

const projetos = [
  {
    title: 'Campus Aberto - Atlética Panterão',
    members: [
      {
        name: 'Marcelo Teixeira de Sousa Filho',
        role: 'Bolsista de Extensão - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/marcelo',
        github: 'https://github.com/marcelo',
      },
      {
        name: 'Isabelly Araujo Temoteo',
        role: 'Bolsista de Extensão - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/marcelo',
        github: 'https://github.com/marcelo',
      },
      {
        name: 'Marcelo Teixeira',
        role: 'Bolsista de Extensão - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/marcelo',
        github: 'https://github.com/marcelo',
      },
      {
        name: 'Marcelo Teixeira',
        role: 'Bolsista de Extensão - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/marcelo',
        github: 'https://github.com/marcelo',
      },
      // ...outros membros
    ],
  },
  {
    title: 'Campus Aberto - Runners',
    members: [
      {
        name: 'Joana Costa',
        role: 'Voluntária - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/joana',
        github: 'https://github.com/joana',
      },
      {
        name: 'Joana Costa',
        role: 'Voluntária - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/joana',
        github: 'https://github.com/joana',
      },
      {
        name: 'Joana Costa',
        role: 'Voluntária - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/joana',
        github: 'https://github.com/joana',
      },
      {
        name: 'Joana Costa',
        role: 'Voluntária - 2025',
        image: gabriela,
        linkedin: 'https://linkedin.com/in/joana',
        github: 'https://github.com/joana',
      },
      // ...outros membros
    ],
  },
];
</script>

<template>
    <div class="flex flex-col items-center">
        <!-- Banner -->
        <BannerParticipantes />

        <!-- Placeholder do slider -->
        <div class="flex justify-center items-center mt-20 mb-20 w-1/2">
        <Carousel />
        </div>

        <!-- Faixa laranja -->
        <div class="h-10 bg-orange-500"></div>

        <!-- Seções de projetos -->
        <div class="bg-white w-screen">
            <div class="container mx-auto px-4 py-16">
                <ProjectSection
                v-for="(projeto, index) in projetos"
                :key="index"
                :title="projeto.title"
                :members="projeto.members"
                />
            </div>
        </div>

        <!-- Faixa laranja final -->
        <div class="h-10 bg-orange-500"></div>
    </div>
</template>
