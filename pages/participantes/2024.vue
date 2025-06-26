<template>
    <div class="flex flex-col">
      <BannerParticipantes />
      <div class="flex justify-center mt-20 mb-20 w-full">
        <div class="w-1/2">
          <Carousel />
        </div>
      </div>
      <!-- faixa -->
      <div class="h-10 bg-orange-500"></div>
      <div class="bg-white">
        <div class="container mx-auto px-4 py-16">
          <ProjectSection
            v-for="(projeto, index) in projetos"
            :key="index"
            :title="projeto.title"
            :members="projeto.members"
            />
        </div>
      </div>
      <!-- faixa -->
      <div class="h-10 bg-orange-500"></div>
    </div>
</template>

<script setup>
  import BannerParticipantes from '@/components/Participantes/BannerParticipantes.vue';
  import ProjectSection from '@/components/Participantes/ProjectSection.vue';

  //imports de imagens para os cards
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
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
        {
          name: 'Isabelly Araujo Temoteo',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
        {
          name: 'Marcelo Teixeira',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
        {
          name: 'Marcelo Teixeira',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
      ],
    },
    {
      title: 'Campus Aberto - Runners',
      members: [
        {
          name: 'Joana Costa',
          role: 'Voluntária - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Joana Costa',
          role: 'Voluntária - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Joana Costa',
          role: 'Voluntária - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Joana Costa',
          role: 'Voluntária - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
  ];
</script>