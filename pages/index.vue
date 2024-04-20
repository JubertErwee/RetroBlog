<script setup>
import {ref} from 'vue';
import Cards from '../components/Cards';
const cardData = ref([
  { id: 1, title: 'Doctor Strange', content: '"Doctor Strange in the Multiverse of Madness" explores the multiverse as Doctor Strange faces new threats and delves deeper into the mystical realms to confront dark forces.', image: '/img/blog3.jpg' },
  { id: 2, title: 'Avengers: Endgame', content: '"Avengers: Endgame" follows Earth\'s mightiest heroes as they embark on a time-bending mission to reverse the devastating effects of Thanos\' snap and restore order to the universe.', image: '/img/blog-1.jpg' },
  { id: 3, title: 'Black Panther', content: '"Black Panther" follows T\'Challa, the newly crowned king of Wakanda, as he grapples with his new role while confronting internal and external threats to his kingdom\'s peace and prosperity.', image: '/img/blog4.jpeg' }
]);

const version = 2 + 1
</script>

<template>
  <header>
      <h1>RetroBlog</h1>
      <nav>
        <ul class="nav">
          <li class="nav-item">
            <button type="button" class="btn btn-danger"><nuxt-link to="/" exact>Home</nuxt-link></button>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-warning"><nuxt-link to="/about">About</nuxt-link></button>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-primary"><nuxt-link to="/contact">Contact</nuxt-link></button>
          </li>
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
  :image="data.image"
  :title="data.title"
  :content="data.content"></Cards>
  <Cards
  v-for="data in cardData"
  :key="data.id"
  :image="data.image"
  :title="data.title"
  :content="data.content"></Cards>
  <Cards
  v-for="data in cardData"
  :key="data.id"
  :image="data.image"
  :title="data.title"
  :content="data.content"></Cards>
</div>
</div>
</template>

<style>
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
