<script setup>
defineProps(['title', 'content']);
</script>

<template>
  <div class="col-md-4 my-3 mx-auto">
    <div class="card p-4">
    <img alt="Avatar" style="width:100%">
    <div class="container">
      <h4>{{ title }}</h4>
      <p>{{ content }}</p>
    </div>
</div>
</div>
</template>


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
  
  
  </style>
  