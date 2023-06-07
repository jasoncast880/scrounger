<template>
  <div class="container">
    <h2>Login</h2>
    <div>
      <form @submit="login">
        <p>
          <label for="username">Username</label>
        </p>
        <p >
          <input class = "submission-field" type="text" id="username" v-model="username" required>
        </p>
        <p>
          <label for="password">Password</label>
        </p>
        <p>
          <input type="password" id="password" v-model="password" required>
        </p>
        <p class="btn-component">
          <Button
            @btn-click="$emit('toggle-add-task')"
            :text="'Login'"
          />

          <a href="url">Forgot Password</a>
        </p>

        
      </form>
    </div>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
  name: 'SignInForm',
  props: {
  },
  components:{
    Button,
  },
  // data() {
  //   return {
  //     username: '',
  //     password: '',
  //   };
  // },
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
  a{font-size:12px}
/* 
	form  { display: table;      }
	p     { display: table-row;  }
	label { display: table-cell; }
	input { display: table-cell; } */
  .container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 450px;
    height: 300px;
    border-radius: 10px;
    border-color: #999999;
    border-style: solid;
    border-width: 1px;
    background-color: #ffffff;
  }
  .btn-component{
    margin: 0;
    left:50%;
    display:inline-block;
  }

/*style logic here*/
</style>