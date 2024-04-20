<script setup>
defineProps(['title', 'content', 'image']);
</script>

<template>
    <div class="col-md-4 my-3 mx-auto">
      <div class="card p-4">
      <img :src="`${image}`" class="card-img-top">
      <div class="card-body">
        <h4>{{ title }}</h4>
        <p>{{ content }}</p>
      </div>
      </div>
    </div>
</template>

  <style scoped>
  h4{
    color: #4d9c65;
  }

  .card{
    background: #eef1ee;
  }
  .container {
    font-family: Arial, Helvetica, sans-serif;
    width: 100%;
  }
  
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
  