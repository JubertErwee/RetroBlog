<template>
  <div class="container text-center">
    <div class="row">
      <div class="col"></div>
      <div class="col">
        <h2 class="text-center mb-4">Contact Us</h2>
        <form id="myform" @submit.prevent="submitForm">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" v-model="name" class="form-control" id="name" placeholder="Enter your name">
          </div>
          <div class="form-group">
            <label for="email">Email address</label>
            <input type="email" v-model="email" class="form-control" id="email" placeholder="Enter your email">
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea v-model="message" class="form-control" id="message" rows="5" placeholder="Enter your message"></textarea>
          </div>
          <button type="submit" id="btnSubmit" class="btn btn-primary btn-block">Submit</button>
        </form>
        <div v-if="showPopup" class="alert alert-danger mt-3" role="alert">
          Not all fields entered info!
        </div>
      </div>
      <div class="col"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      message: '',
      showPopup: false
    };
  },
  methods: {
    submitForm() {
      if (!this.name || !this.email || !this.message) {
        this.showPopup = true;
      } else {
        // Redirect logic
        // For now, let's just log the form data
        console.log('Name:', this.name);
        console.log('Email:', this.email);
        console.log('Message:', this.message);

        // Redirect back to '/'
        // You can replace this with your actual redirection logic
        window.location.href = '/';
      }
    }
  }
};
</script>

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
</style>
