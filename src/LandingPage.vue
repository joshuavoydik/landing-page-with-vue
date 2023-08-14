<template>
  <div class="container">
    <h1>Welcome to the Daily Build project for August 15th </h1>
    <p>Subscribe to stay updated with our latest news!</p>
    <input type="email" v-model="email" placeholder="Your email address" />
    <button @click="subscribe">Subscribe</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: ''
    };
  },
  methods: {
    subscribe() {
      if (this.email) {
        // Add your subscription logic here
        alert('Thank you for subscribing!');
      } else {
        alert('Please enter a valid email address.');
      }
    }
  }
};
</script>

<style scoped>
.container {
  font-family: 'Inter', serif; /* Example of a serif font */
  background-color: #f9bebe; /* Soft red */
  padding: 40px 20px 50px;
  text-align: center;
  max-width: 600px;
  margin: 0 auto; /* Removed top and bottom margin */
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
}
h1 {
  font-size: 2.5rem;
  color: #333;
}
p {
  font-size: 1.2rem;
  color: #555;
}
input {
  width: 80%;
  padding: 10px;
  font-size: 1rem;
  margin: 20px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}
button {
  padding: 10px 20px;
  font-size: 1rem;
  background-color: #ff6969; /* Slightly darker red */
  color: white;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  transition: 0.3s;
}
button:hover {
  background-color: #ff2d2d;
}
</style>
