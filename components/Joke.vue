<template>
   <nuxt-link :to="'jokes/'+id">
      <div class="border border-dotted border-gray-400 p-1 my-1">
         {{joke}}
      </div>
   </nuxt-link>
</template>

<script>
export default {
   name: 'Joke',
   props:{
      joke:{
         type: String,
         required: true
      },
      id:{
         type: String,
         required: true
      },
   }
}
</script>