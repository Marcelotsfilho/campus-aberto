<template>
    <div class="flex flex-col">
        <div class="bg-black">
            <BannerProjetos />
        </div>
        <div class="flex flex-row items-center mt-10 bg-[#000136] rounded-4xl p-10 mx-15">
            <div class="flex flex-col ml-10">
                <h1 class="text-3xl font-bold mb-5 text-orange-500 justify-start">
                    CAMPUS ABERTO
                </h1>
                <h1 class="text-3xl font-bold mb-5 text-white">OFICINAS ESPORTIVAS</h1>
                <p class="flex justify-center text-lg text-white mb-5 w-3xl text-justify">
                    O Campus Aberto é núcleo formado por um grupo de discentes (bolsistas
                    e voluntários) de diferentes níveis de ensino (técnico, graduação e
                    pós-graduação) regularmente matriculados no campus Leopoldina, que
                    desenvolvem ações de ensino, pesquisa e extensão no contexto do
                    Esporte, coordenados pela professora de Educação Física, Gabriela
                    Venturini. Dessa forma, a Atlética CEFET Leopoldina, também conhecida
                    como Atlética Panterão, funciona como um “braço” do Campus Aberto,
                    que tem como objetivo, representar o CEFET-MG em competições
                    esportivas e promover a aproximação do Campus Leopoldina da
                    comunidade através do esporte, em diferentes contextos: educacional,
                    científico, acadêmico, tecnológico, de saúde e lazer.
                </p>
                <p class="text-white">
                    Disponível em:
                    <a
                    href="https://atletica-panterao-leopoldina.netlify.app/"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="text-orange-400 hover:underline"
                    >
                    https://atletica-panterao-leopoldina.netlify.app/
                    </a>
                </p>
            </div>
            <div class="flex flex-col justify-center ml-25">
                <img
                    src="/assets/images/futsal.png"
                    alt="Oficinas Esportivas"
                    class=""
                />
            </div>
        </div>

        <div class="flex items-start justify-center gap-30 mt-20">
            <div class="">
                <TotemProjects
                    titulo="CAMPUS ABERTO RUNNERS"
                    :imagem="runnerImg"
                    :descricao="descricao"
                    link="https://atletica-panterao-leopoldina.netlify.app/campus-aberto-runners"
                />
            </div>
            <div class="">
                <TotemProjects
                    titulo="CAMPUS ABERTO ARTE, CULTURA E TECNOLOGIA"
                    :imagem="runnerImg"
                    :descricao="descricaoRunners"
                    link="https://atletica-panterao-leopoldina.netlify.app/campus-aberto-runners"
                />
            </div>
        </div>

    </div>
</template>
  
<script setup>
  import BannerProjetos from '~/components/BannerProjetos.vue'
  import TotemProjects from '~/components/TotemProjects.vue'
  import runnerImg from '~/assets/images/futsal.png'
  
    const descricao = [
        `O Campus Aberto é núcleo formado por um grupo de discentes (bolsistas e voluntários)
        de diferentes níveis de ensino (técnico, graduação e pós-graduação) regularmente
        matriculados no campus Leopoldina, que desenvolvem ações de ensino, pesquisa e
        extensão no contexto do Esporte, coordenados pela professora de Educação Física,
        Gabriela Venturini. Dessa forma, a Atlética CEFET Leopoldina, também conhecida como Atlética Panterão,
        funciona como um “braço” do Campus Aberto, que tem como objetivo representar o CEFET-MG
        em competições esportivas e promover a aproximação do Campus Leopoldina da comunidade
        através do esporte, em diferentes contextos: educacional, científico, acadêmico,
        tecnológico, de saúde e lazer.`
    ]
    const descricaoRunners = [
        `Descrição dos Runners`
    ]
</script>
  