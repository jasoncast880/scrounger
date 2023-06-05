<template>
  <div class="container" id="app">
    <div class = "centered-component">
      <SignInForm />
    </div>
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
body {
  font-family: 'Poppins', sans-serif;
  
}
.container {
  position: fixed;
  top:0;
  left:0;
  right:0;
  bottom:0;
  width: 100%;
  height: 100%;
  z-index: 9999;
  background: #181818;
  color: #CCCC00;
}
.centered-component{
  display: flex;
  justify-content: center;
  align-items: center;
  height:90vh;
}
</style>