<script setup lang="ts">
const posts = [
  { id: 1, title: 'First Post', content: 'This is the content of the first post.' },
  { id: 2, title: 'Second Post', content: 'This is the content of the second post.' },
  { id: 3, title: 'Third Post', content: 'This is the content of the third post.' }
];

const version = 2 + 1
</script>

<template>
<div class="cards-row">
    <div class="card">
    <img alt="Avatar" style="width:100%">
    <div class="container">
      <h4><b class="cardsname">John Doe</b></h4>
      <p class="cardsname">Architect & Engineer</p>
    </div>
  </div>
  <div class="card">
    <img alt="Avatar" style="width:100%">
    <div class="container">
      <h4><b class="cardsname">John Doe</b></h4>
      <p>Architect & Engineer</p>
    </div>
  </div>
  <div class="card">
    <img alt="Avatar" style="width:100%">
    <div class="container">
      <h4><b class="cardsname">John Doe</b></h4>
      <p>Architect & Engineer</p>
    </div>
  </div>
</div>
  </template>
  <style scoped>
  .container {
    font-family: Arial, Helvetica, sans-serif;
    width: 100%;
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
  
  /*  the code for the card styling begins here */
  
  .cards-row {
    display: flex;
    flex-direction: row;
    justify-content: space-between; /* Distribute items evenly along the main axis */
  }
  .card {
    /* Add shadows to create the "card" effect */
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    width: 30%; /* Set width to 30% to display three cards next to each other */
    margin: 20px;
    background-color: #c2c7c4;
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
  
  </style>
  