<template>
    <header class="flex flex-row items-center justify-between bg-white p-4 pr-32 w-full">
        <nuxt-link to="/">
            <img src="/assets/images/logoC.A-azul.png" alt="Logo" class="h-10 w-auto pl-10" />
        </nuxt-link>
        <nav class="flex space-x-20">
            <nuxt-link to="/" class="text-black hover:text-orange-300 text-xl">Home</nuxt-link>
            <nuxt-link to="/projetos" class="text-black hover:text-orange-300 text-xl">Projetos</nuxt-link>
            <nuxt-link to="/modalidades" class="text-black hover:text-orange-300 text-xl">Modalidades</nuxt-link>
        </nav>
    </header>
</template>
