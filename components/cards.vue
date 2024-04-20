<script setup>
defineProps(['title', 'content']);
</script>

<template>

<div class="cards-row">
    <div class="col-md-4 my-3 mx-auto">
      <div class="card p-4">
      <img alt="Avatar" style="width:100%">
      <div class="container">
        <h4>{{ title }}</h4>
        <p>{{ content }}</p>
      </div>
      </div>
    </div>
    <div class="card">
    <img  src="..\components\assets\blog3.jpg" alt="Avatar" style="width:100%">
    <div class="container">
      <h4>{{ data[0].title }}</h4>
      <p>{{ data[0].content}}</p>
      <h4><b class="cardsname">Doctor Strange</b></h4>
      <p class="pdiscript">Doctor Strange offers a visually stunning and mind-bending journey into the mystical realms, with impressive performances and inventive storytelling."r</p>
    </div>
  <div class="card">
    <img src="..\components\assets\blog-1.jpg" alt="Avatar" style="width:100%">
    <div class="container">
      <h4><b class="cardsname">Avengers </b></h4>
      <p class="pdiscript">Architect & Engineer</p>
    </div>
  <div class="card">
    <img src="..\components\assets\blog4.jpeg" alt="Avatar" style="width:100%">
    <div class="container">
      <h4><b class="pdiscript">Black Panther</b></h4>
      <p>Architect & Engineer</p>
    </div>
</div>
  <style scoped>
  .container {
    font-family: Arial, Helvetica, sans-serif;
    width: 100%;
  }

  <style scoped>
  
  p {
    font-size: 1.2rem;
    color: #666;
  }
  
  .btn:hover {
    background-color: #555;
  }

  /* On mouse-over, add a deeper shadow */
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }
  
  /* Add some padding inside the card container */
  .container {
    padding: 2px 16px;
  }
  .cardsname{
    color: #4d9c65;
  }
  .pdiscript{
    color: #eef6ee;
  }
  
  </style>
  