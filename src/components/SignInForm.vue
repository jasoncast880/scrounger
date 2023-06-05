<template>
  <div class="sign-on-box">
    <h2 align="center">Login</h2>
    <form @submit="login">
      <p>
        <label for="username">Username&#9&nbsp</label>
        <input type="text" id="username" v-model="username" required>
      </p>
      <p>
        <label for="password">Password</label>
        <input type="password" id="password" v-model="password" required>
      </p>
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
  data() {
    return {
      username: '',
      password: '',
    };
  },
  methods: {
    login(event) {
      event.preventDefault();
      // Add your login logic here
      console.log('Username:', this.username);
      console.log('Password:', this.password);
    },
  },
};
</script>

<style scoped>
	form  { display: table;      }
	p     { display: table-row;  }
	label { display: table-cell; }
	input { display: table-cell; }
/*style logic here*/
</style>