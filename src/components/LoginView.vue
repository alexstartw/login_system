<template>
  <form name="login-form" >
    <div class="mb-3">
      <label for="username">Username: </label>
      <input type="text" id="username" v-model="input.username" />
    </div>
    <div class="mb-3">
      <label for="password">Password: </label>
      <input type="password" id="password" v-model="input.password" />
    </div>
    <button class="btn btn-outline-dark" type="submit">
      Login
    </button>

    <button class="btn btn-outline-dark" type="submit">
      Register
    </button>

    <p>Username is: {{input.username}}</p>
    <p>Password is: {{input.password}}</p>
  </form>
</template>

<script>
export default {
  name: 'LoginView',
  data(){
    return{
      input:{
        username: "",
        password: ""
      }
    }
  }
}
</script>