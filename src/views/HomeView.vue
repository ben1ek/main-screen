<template>
  <div class="container">
    <div class="main-screen-content">
      <v-img class="main-screen-image" :src="require('../assets/main-screen-image.svg')" contain/>
      <p class="text-center caption-text">Welcome</p>
      <h1>
        <v-img class="main-logo-image" :src="require('../assets/teamo-logo.svg')" contain/>
      </h1>
      <p class="text-center caption-text">Same & Next-Day Delivery of <br>large packages</p>
      <v-btn class="start-button font-weight-regular" x-large elevation="0">Start Now</v-btn>
    </div>
      <div class="login-container">
        <p>Already have an account?&nbsp;</p>
        <router-link to="/login">About</router-link>
      </div>
  </div>
</template>

<script>
  export default {
    name: 'HomeView',
    components: { },
  }
</script>

<style>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100%;
  background-color: #F5F5F5;
  /* font-family: 'Kamerik 105'; */
}
.main-screen-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.main-logo-image {
  max-width: 90vw;
}
.main-screen-image {
  max-height: 290px;
  max-width: 90vw;
  margin-top: 8vh;
  margin-bottom: 2vh;
}
.caption-text {
  padding: 20px 0;
  margin-bottom: 0 !important;
  font-size: 16px;
  color: #3B4F41;
}
.start-button {
  color: #0A2B14;
  background-color: #E6F40A !important;
  max-width: 340px;
  width: 100%;
  border-radius: 12px;
  letter-spacing: 0.08em;
  margin-bottom: 20px;
}
.start-button:hover, .start-button:focus, .start-button::before {
  background-color: #EFFF00 !important;
}
.login-container {
  display: flex;
  justify-content: center;
  margin-top: auto;
  margin-bottom: 4vh;
}
.login-container a {
  color: #07872E !important;
}
.v-ripple__container {
  display: none;
}
</style>