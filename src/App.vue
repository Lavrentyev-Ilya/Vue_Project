<template>
<<<<<<< HEAD
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
=======
  <div>
    <button v-on:click="addLikes">Likes</button>
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
>>>>>>> 661c6fe (init)
