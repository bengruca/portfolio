<template>
  <main class="min-h-screen">
    <section class="py-20 px-6 md:px-20 bg-gradient-to-b from-gray-900 to-gray-800 text-center">
      <h1 class="text-4xl md:text-6xl font-bold mb-4">Hi, I'm Ben Gruca</h1>
      <p class="text-lg md:text-xl text-gray-300 mb-6">
        Graduate Student at University of Southern California
      </p>
      <button class="bg-white text-black px-4 py-2 rounded">View My Work</button>
    </section>

    <section class="py-20 px-6 md:px-20">
      <h2 class="text-3xl font-semibold mb-12 text-center">Image Gallery</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        <img v-for="n in 6" :key="n" :src="'https://source.unsplash.com/600x400?tech&sig=' + n" class="w-full h-60 object-cover rounded-xl" />
      </div>
    </section>

    <section class="py-20 px-6 md:px-20 bg-gray-900 text-center">
      <h2 class="text-3xl font-semibold mb-6">Let’s Connect</h2>
      <p class="text-gray-400 mb-6">Available for freelance, full-time, and collaborations.</p>
      <button class="bg-white text-black px-4 py-2 rounded">Email Me</button>
    </section>
  </main>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
</style>