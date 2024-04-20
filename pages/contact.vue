<template>
  <div class="container text-center">
    <div class="row">
      <div class="col"></div>
      <div class="col">
        <h2 class="text-center mb-4">Contact Us</h2>
        <form>
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" class="form-control" id="name" placeholder="Enter your name">
          </div>
          <div class="form-group">
            <label for="email">Email address</label>
            <input type="email" class="form-control" id="email" placeholder="Enter your email">
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea class="form-control" id="message" rows="5" placeholder="Enter your message"></textarea>
          </div>
          <button type="submit" id="btnSubmit" class="btn btn-primary btn-block">Submit</button>
        </form>
      </div>
      <div class="col"></div>
    </div>
  </div>

  <footer class="footer bg-dark text-light py-4">
    <div class="container text-center">
      <div class="row">
        <div class="col-md-4">
          <h5>Location</h5>
          <p><i class="fas fa-map-marker-alt"></i> 123 Main Street, City, Country</p>
        </div>
        <div class="col-md-4">
          <h5>Call</h5>
          <p><i class="fas fa-phone"></i> +1234567890</p>
        </div>
        <div class="col-md-4">
          <h5>Email</h5>
          <p><i class="fas fa-envelope"></i> contact@example.com</p>
        </div>
      </div>
    </div>
  </footer>

  
</template>
<style scoped>
      .container {
    width: 100%;
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-group label {
      text-align: left; 
      display: block;
      width: 100%;
    }

    .btn btn-primary btn-block
    {

    }

  </style>