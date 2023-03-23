<template>
  <h1>Posts</h1>
  <div class="card p-3 m-3" style="width: max-content; margin: auto">
    <form class="custom-form" @submit.prevent="addPost">
      <div class="form-group">
        <label for="userId" >User Id</label>
        <input type="text" class="custom-form-control" id="userId" v-model="posts.userId">
      </div>
      <div class="form-group">
        <label for="title" >Title</label>
        <input type="text" class="custom-form-control" id="title" v-model="posts.title">
      </div>
      <div class="form-group">
        <label for="body" >Content</label>
        <textarea class="custom-form-control" id="body" row="5" col="20" v-model="posts.body"></textarea>
      </div>
      <button type="submit" class="btn btn-outline-primary">Add Post</button>
    </form>
  </div>   
</template>

<script>

    export default {
    data() {
      return {
        posts: {
          userId: '',
          title: '',
          body: '',
        }
      }
    },
    methods: {
      addPost() {
        fetch('https://jsonplaceholder.typicode.com/posts/', {
          method: 'POST',
          headers: {
            'content-type': 'applications/json'
          },
          body: JSON.stringify({
            userId: this.userId,
            title: this.title,
            body: this.body,
          })
        })
        .then(response => response.json())
        .then(data => console.log(data))
      }
    }
  }
</script>

<style scoped>
  label {
    display: block;
  }
</style>