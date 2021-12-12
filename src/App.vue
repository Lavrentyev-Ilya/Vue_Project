<template>
<div>
    <button v-on:click="addLikes">Likes6</button>
    <button v-on:click="addDislikes">Dislikes</button>
  </div>
  <div>Количество Likes <strong>{{ likes }}</strong></div>
  <div>Количество Likes <strong>{{ dislikes }}</strong></div>
</template>

<script>
  export default {
    data(){
      return{
        likes: 0,
        dislikes: 5,
      }
    },
    methods: {
      addLikes(){
        this.likes++
      },
      addDislikes(){
        this.dislikes++
      }
    }
  }
</script>

<style>

</style>
