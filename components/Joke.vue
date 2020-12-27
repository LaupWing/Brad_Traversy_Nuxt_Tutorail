<template>
   <div class="border border-dotted border-gray-400 p-1 my-1">
      {{joke}}
   </div>
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
         type: Number,
         required: true
      },
   }
}
</script>