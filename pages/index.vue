<script setup>
import {ref} from 'vue';
import Cards from '../components/Cards.vue';
const cardimages = ref([
  { content: 'This is the content of the first post.' },
  { content: 'This is the content of the second post.' },
  { content: 'This is the content of the third post.' }
]);

const cardData = ref([
  { id: 1, title: 'First Post', content: 'This is the content of the first post.' },
  { id: 2, title: 'Second Post', content: 'This is the content of the second post.' },
  { id: 3, title: 'Third Post', content: 'This is the content of the third post.' },
  { id: 4, title: 'Fourth Post', content: 'This is the content of the fourth post.' },
  { id: 5, title: 'Fifth Post', content: 'This is the content of the fifth post.' },
  { id: 6, title: 'Sixth Post', content: 'This is the content of the sixth post.' },
  { id: 1, title: 'First Post', content: 'This is the content of the first post.' },
  { id: 2, title: 'Second Post', content: 'This is the content of the second post.' },
  { id: 3, title: 'Third Post', content: 'This is the content of the third post.' },
  { id: 4, title: 'Fourth Post', content: 'This is the content of the fourth post.' },
  { id: 5, title: 'Fifth Post', content: 'This is the content of the fifth post.' },
  { id: 6, title: 'Sixth Post', content: 'This is the content of the sixth post.' }
]);
</script>

<template>
  <header>
      <h1>Retro blog </h1>
      <nav>
        <ul class="nav">
          <li class="nav-item">
            <button type="button" class="btn btn-danger"><nuxt-link to="/" exact>Home</nuxt-link></button>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-warning"><nuxt-link to="/about">About</nuxt-link></button>
          </li>
          <!-- Add more navigation links here -->
        </ul>
      </nav>
    </header>
  <div class="container my-3">
    
 <!-- the code for the card begings here -->
  
<!-- first part ends here , -->
<div class="row overflow-x-hidden">
  <Cards
  v-for="data in cardData"
  :key="data.id"
  :title="data.title"
  :content="data.content"></Cards>
</div>

</div>
</template>

<style scoped>
.container {
  font-family: Arial, Helvetica, sans-serif;
  width: 100%;
}

header {
  background-color: #333;
  color: #4d9c65;
  padding: 20px 0;
}

header h1 {
  font-size: 2.5rem;
  margin-left: 20px;
}

.nav {
  display: flex;
  justify-content: center;
  list-style: none;
  padding: 0;
}

.nav-item {
  margin-right: 10px;
}

.nav-item:last-child {
  margin-right: 0;
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

/* On mouse-over, add a deeper shadow */
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}


</style>
