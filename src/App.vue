<template>
  <div class="app">
    <form>
      <input class="input" type="text" placeholder="Название">
      <input class="input" type="text" placeholder="Описание">
      <button class="btn" @click="createPost">Create post</button>
    </form>
    <div class="post" v-for="post in posts" v-bind:key="post.id">
      <div><strong>Название</strong> {{post.title}}</div>
      <div><strong>Описание</strong> {{post.body}}</div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      posts: [
        {id: 1, title: 'Behappy Eng', body: 'Описание - 1'},
        {id: 2, title: 'Behappy Eng', body: 'Описание - 2'},
        {id: 3, title: 'Behappy Eng', body: 'Описание - 3'},
        {id: 4, title: 'Behappy Eng', body: 'Описание - 4'}
      ]
    }
  },
  methods: {
    createPost(){
      this.posts.push({id: 5, title: 'Behappy Eng', body: 'Описание - 5'})
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  padding: 20px;
}
.post{
  padding: 15px;
  border: 3px solid #0a6c41;
  margin-top: 15px;
}
form{
  display: flex;
  flex-direction: column;
}
.input{
  width: 50%;
  border: 1px solid coral;
  padding: 10px 15px;
  margin-top: 10px;
}
.btn{
  margin-top: 10px;
  align-self: flex-end;
  padding: 10px 15px;
  background: none;
  border: 2px solid #0a6c41;
}
</style>
