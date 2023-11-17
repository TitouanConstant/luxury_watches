<template>
  <div class="form-container">
    <h1>Create Your Account</h1>
    <form @submit.prevent="register">
      <input type="text" class="form-input" placeholder="First Name" v-model="user.firstName" required />
      <input type="text" class="form-input" placeholder="Last Name" v-model="user.lastName" required />
      <input type="email" class="form-input" placeholder="Email" v-model="user.email" required />
      <input type="date" class="form-input" placeholder="Birthdate" v-model="user.birthdate" required />
      <input type="password" class="form-input" placeholder="Password" v-model="user.password" required />
      <input type="password" class="form-input" placeholder="Confirm Password" v-model="confirmPassword" required />
      <button type="submit" class="form-button">Register</button>
    </form>
  </div>
</template>
<script>
export default {
  data () {
    return {
    }
  }
}
</script>
<style>
.form-container {
    max-width: 400px;
    margin: 50px auto;
    padding: 20px;
    text-align: center;
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
    transition: all 0.3s ease-in-out;
  }
  .form-container:hover {
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
  }
  .form-input {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border: 1px solid #bbb;
    border-radius: 5px;
    box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.1);
    transition: border-color 0.3s;
  }
  .form-input:focus {
    border-color: #333;
    outline: none;
    box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2), 0 0 5px rgba(51, 51, 51, 0.5);
  }
  .form-button {
    width: 100%;
    padding: 12px;
    margin-top: 10px;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1em;
    transition: background-color 0.3s;
  }
  .form-button:hover {
    background-color: #444;
  }
  .form-footer {
    margin-top: 20px;
  }
  .form-footer a {
    color: #333;
    text-decoration: none;
  }
  .form-link {
    display: block;
    margin-bottom: 10px;
  }
  h1 {
    font-size: 2em;
    margin-bottom: 10px;
    color: #333;
  }
  p {
    color: #666;
  }
</style>
