
<script setup lang="ts">
const posts = [
  { id: 1, title: 'First Post', content: 'This is the content of the first post.' },
  { id: 2, title: 'Second Post', content: 'This is the content of the second post.' },
  { id: 3, title: 'Third Post', content: 'This is the content of the third post.' }
];

const version = 2 + 1
</script>

<template>
  <div class="container">
    <header>
      <h1>Retro blog </h1>
      <nav>
        <ul>
          <button type="button" class="btn btn-danger">Home</button>
          <button type="button" class="btn btn-warning">About</button>
          <li><nuxt-link to="/" exact>Home</nuxt-link></li>
          <li><nuxt-link to="/about">About</nuxt-link></li>
          <!-- Add more navigation links here -->
        </ul>
      </nav>
    </header>
    <div class="blog">
      <ul>
        <li v-for="post in posts" :key="post.id" class="post">
          <h2>{{ post.title }}</h2>
          <p>{{ post.content }}</p>
          <nuxt-link :to="'/post/' + post.id" class="btn">Read More</nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.container {
  font-family: Arial, Helvetica, sans-serif;
}

header {
  background-color: #333;
  color: #fff;
  padding: 20px 0;
}

header h1 {
  font-size: 2.5rem;
  margin-left: 20px;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin-top: 10px;
}

nav ul li {
  display: inline;
  margin-right: 20px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
  font-size: 1.2rem;
}

.blog {
  padding: 20px;
}

.post {
  margin-bottom: 20px;
}

h2 {
  font-size: 2rem;
  margin-bottom: 10px;
}

p {
  font-size: 1.2rem;
  color: #666;
}

.btn {
  display: inline-block;
  background-color: #333;
  color: #fff;
  padding: 10px 20px;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s;
}

.btn:hover {
  background-color: #555;
}
</style>
