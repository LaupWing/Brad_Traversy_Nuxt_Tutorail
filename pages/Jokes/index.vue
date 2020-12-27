<template>
   <div>
      Jokes 
   </div>
</template>

<script>
import axios from 'axios'

export default {
   data(){
      return{
         jokes: []
      }
   },
   async created(){
      const config = {
         headers:{
            'Accept': 'application/json'
         }
      }
      try{
         const res = await axios.get('https://icanhazdadjoke.com/search', config)
         const json = await res.json()
         console.log(json)
      }catch(e){
         console.log(e)
      }

   },
   head(){
      return{
         title: 'Dad Jokes',
         meta:[
            {
               hid: 'description',
               name: 'description',
               content: 'Best place for corny dad jokes'
            }
         ]
      }
   }
}
</script>