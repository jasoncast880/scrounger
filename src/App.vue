<template>
  <div class="flex-wrapper">
    <div id="header-id"><Header/></div>

    <div class="center" id="form-id">
      <!-- re-add ceter class -->
      <SignInForm />
    </div>

    <div id="footer-id"><Footer/></div>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import SignInForm from './components/SignInForm.vue';
  import Footer from './components/Footer.vue';
  export default{
    name: 'App',
    components:{
      SignInForm,
      Header,
      Footer,
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
/* .container {
  position: fixed;
  
  background: #f7f5f5;
  color: #181818;
} */
.center {
  display:flex;
  justify-content: center;
  align-items: center;
}
.flex-wrapper{
    display:flex;
    flex-direction:column;
    height: 100vh;
    z-index: 9999;
}

#form-id{
  margin-top:40px;
  margin-bottom:20px;
}

#footer-id{
  margin-top:auto;
}
</style>