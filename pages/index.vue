<template>
    <div>
        <Banner />
        <div class="flex justify-center mt-40">
            <About />
        </div>
        <div class="mt-40">
            <Projects />
        </div>
    </div>
</template>

<script setup>
    import About from '~/components/Home/About.vue'
    import Projects from '~/components/Home/Projects.vue'
</script>