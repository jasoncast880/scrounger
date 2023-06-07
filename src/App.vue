<template>
  <div class = "center">
    <SignInForm />
  </div>
</template>

<script>
  import SignInForm from './components/SignInForm.vue';

  export default{
    name: 'App',
    components:{
      SignInForm,
    },
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
main {
  background-image: url('./assets/banner.jpg');
  background-size: cover;
}
body {
  font-family: 'Poppins', sans-serif;
  
}
/* .container {
  position: fixed;
  top:0;
  left:0;
  right:0;
  bottom:0;
  width: 100%;
  height: 100%;
  z-index: 9999;
  background: #f7f5f5;
  color: #181818;
} */
.center {

  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>