<template>
  <main class="main">
    <section class="register">
      <div class="container">
        <h1 class="register__title">Login to NNGROUP</h1>
        <div class="register__inner">
          <form class="register__form">
            <p class="register__form-text">Please fill out this fields</p>
            <div class="register__form-group">
              <label for="name">Name</label>
              <input id="name" placeholder="Name" type="text">
            </div>
            <div class="register__form-group">
              <label for="email">Email</label>
              <input id="email" placeholder="Email" type="text">
            </div>
            <div class="register__form-group">
              <label for="password">Password</label>
              <input id="password" placeholder="Password" type="text">
            </div>
            <div class="register__form-group">
              <label for="password-confirm">Confirm password</label>
              <input id="password-confirm" placeholder="Confirm password" type="text">
            </div>
          </form>
        </div>
      </div>
    </section>
  </main>
</template>

<style scoped>

  .register {
    padding-top: 50px;
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

</style>
