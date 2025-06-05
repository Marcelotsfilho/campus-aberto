<template>
  <header class="flex flex-row items-center justify-between bg-white px-10 py-4 w-full shadow">
    <nuxt-link to="/" class="flex items-center">
      <img src="/assets/images/logoC.A-azul.png" alt="Logo" class="h-10 w-auto" />
    </nuxt-link>

    <nav class="flex space-x-10 relative text-xl font-medium">
      <nuxt-link to="/" class="text-black hover:text-orange-400 transition">Home</nuxt-link>

      <div class="group relative">
        <span class="text-black hover:text-orange-400 cursor-pointer transition">Participantes</span>

        <div
          class="absolute
                  left-0 
                  mt-2 
                  w-56 
                  bg-white 
                  border 
                  border-gray-200 shadow-lg rounded-md opacity-0 group-hover:opacity-100 group-hover:translate-y-0 transform -translate-y-2 transition-all duration-200 z-50"
        >
            <nuxt-link
              to="/participantes/2024"
              class="block px-4 py-2 text-gray-800 hover:bg-orange-100 transition"
            >
              Campus Aberto 2024
            </nuxt-link>
            <nuxt-link
              to="/participantes/2025"
              class="block px-4 py-2 text-gray-800 hover:bg-orange-100 transition"
            >
              Campus Aberto 2025
            </nuxt-link>
          </div>
        </div>

        <nuxt-link to="/projetos" class="text-black hover:text-orange-400 transition">Projetos</nuxt-link>
        <nuxt-link to="/modalidades" class="text-black hover:text-orange-400 transition">Modalidades</nuxt-link>
      </nav>
  </header>
</template>
