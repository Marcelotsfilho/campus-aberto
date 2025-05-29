<template>
    <div>
      <Header />
      <main class="bg-gradient-to-b from-[#1F2171] to-[#000014] min-h-screen">
        <slot />
      </main>
      <Footer />
    </div>
  </template>
  
  <script setup>
  import Header from '~/components/Header.vue'
  import Footer from '~/components/Footer.vue'
  </script>
  