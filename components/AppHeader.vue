<template>
   <header class="flex justify-between items-center mb-1 pb-1 border-b border-dashed border-gray-400">
      <h1 class="text-blue-400 text-2xl">Dad Jokes</h1>
      <ul class="flex">
         <li class="bg-gray-600 text-white py-1 px-4 m-2">
            <nuxt-link to="/">Home</nuxt-link>
         </li>
         <li class="bg-gray-600 text-white py-1 px-4 m-2">
            <nuxt-link to="/jokes">Jokes</nuxt-link>
         </li>
         <li class="bg-gray-600 text-white py-1 px-4 m-2">
            <nuxt-link to="/about">About</nuxt-link>
         </li>
      </ul>
   </header>
</template>

<script>
export default {
   name: 'AppHeader'
}
</script>