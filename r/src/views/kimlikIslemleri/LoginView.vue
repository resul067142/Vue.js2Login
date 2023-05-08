<template>
  <div class="login-container">
    <div class="login-box">
      <h1 class="login-title">Giriş Yap</h1>
      <form class="login-form">
        <input type="email" placeholder="Email" class="input-field">
        <input type="password" placeholder="Şifre" class="input-field">
        <button class="login-btn" @click.prevent="login">Giriş</button>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  name: "LoginView",
  methods: {
    login() {
      // login işlemi burada gerçekleştirilebilir
    }
  }
}
</script>

<style>
.login-container {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login-box {
  background-color: #f5f5f5;
  padding: 2rem;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  animation-name: login-anim;
  animation-duration: 1s;
  animation-timing-function: ease-in-out;
}

@keyframes login-anim {
  0% {
    opacity: 0;
    transform: translateY(-100px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.login-title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 2rem;
}

.login-form {
  display: flex;
  flex-direction: column;
}

.input-field {
  padding: 1rem;
  margin-bottom: 1rem;
  border: none;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
}

.login-btn {
  background-color: #4caf50;
  color: #fff;
  padding: 1rem;
  border: none;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
  cursor: pointer;
  transition: background-color 0.3s;
}

.login-btn:hover {
  background-color: #3e8e41;
}
</style>
