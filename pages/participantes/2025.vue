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
      title: 'Campus Aberto',
      members: [
        {
          name: 'Pedro Henrique Barbosa',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Jonathan de Assis',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
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
          name: 'Lanna Duarte de Souza',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
        {
          name: 'Isabelly Araujo Temoteo',
          role: 'Voluntária - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/marcelo',
          github: 'https://github.com/marcelo',
        },
      ],
    },
    {
      title: 'Campus Aberto - Arte Cultura e Tecnologia',
      members: [
        {
          name: 'Ítalo Aurélio de Paula Vieira',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Eduarda Costa de Oliveira Silva',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
    {
      title: 'Campus Aberto - Lei de Insentivo ao Esporte',
      members: [
        {
          name: 'Giovana Marreiro Bonin Freire',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Dayana Aparecida Souza Rocha',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
    {
      title: 'Campus Aberto - Runners',
      members: [
        {
          name: 'Kauê Marinato',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Sophia Coura',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
    {
      title: 'Campus Aberto - Educação Física no ENEM',
      members: [
        {
          name: 'Pedro Felipe Eblen',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
        {
          name: 'Rodrigo Venetillo',
          role: 'Bolsista de Extensão - 2025',
          image: gabriela,
          lattes: 'http://lattes.cnpq.br/2523304265479022',
          linkedin: 'https://linkedin.com/in/joana',
          github: 'https://github.com/joana',
        },
      ],
    },
  ];
</script>