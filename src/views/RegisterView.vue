<script setup>
import { ref } from 'vue';

const apiUrl = import.meta.env.VITE_API_URL;

const fields = ref({
  name: "",
  email: "",
  password: "",
  password_confirmation: ""
})

async function register(payload) {
  const res = await fetch(`${apiUrl}/register`, {
    method: 'POST',
    body: JSON.stringify(payload),
    headers: {
      'Content-type': 'application/json',
      'Accept': 'application/json'
    }
  });

  console.log(res);
}
</script>

<template>
  <main class="main">
    <section class="register">
      <div class="container">
        <h1 class="register__title">Login to NNGROUP</h1>
        <div class="register__inner">
          <form @submit.prevent="register(fields)" class="register__form">
            <p class="register__form-text">Please fill out this fields</p>
            <div class="register__form-group">
              <label for="name">Name</label>
              <input v-model="fields.name" id="name" placeholder="Name" type="text">
            </div>
            <div class="register__form-group">
              <label for="email">Email</label>
              <input v-model="fields.email" id="email" placeholder="Email" type="text">
            </div>
            <div class="register__form-group">
              <label for="password">Password</label>
              <input v-model="fields.password" id="password" placeholder="Password" type="text">
            </div>
            <div class="register__form-group">
              <label for="password-confirm">Confirm password</label>
              <input v-model="fields.password_confirmation" id="password-confirm" placeholder="Confirm password" type="text">
            </div>
            <button class="register__form-btn" type="submit">Submit</button>
          </form>
        </div>
      </div>
    </section>
  </main>
</template>

<style scoped>

  .register {
    padding: 50px 0;
  }

  .register__title {
    margin-bottom: 50px;
  }

  .register__inner {
    padding: 30px;
    border-radius: 10px;
    border: 1px solid #212121;
    max-width: 600px;
    margin: 0 auto;
  }

  .register__form-text {
    margin-bottom: 20px;
  }

  .register__form-group {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .register__form-group + .register__form-group {
    margin-top: 20px;
  }

  input {
    height: 40px;
    border-radius: 6px;
    padding: 0 10px;
    border: 1px solid #737373;
  }

  .register__form-btn {
    padding: 10px 15px;
    border-radius: 6px;
    border: none;
    background: #000;
    color: #fff;
    font-family: 'Inter', sans-serif;
    margin: 0 auto;
    margin-top: 40px;
    font-weight: 600;
    cursor: pointer;
    width: 100%;
    max-width: 184px;
    display: block;
  }

</style>
