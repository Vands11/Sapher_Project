<template>
    <div class="login-container">
      <div class="left-panel">
        <!-- Background image will appear here -->
      </div>
      <div class="right-panel">
        <div class="login-card">
          <div class="logo">
            <img src="/img/icons/sapher_logo_with_words.svg" alt="Logo" />
           
          </div>
          <h1>Welcome Back!</h1>
          <p class="subtitle">Please login to your account</p>
          <button @click="handleSSOLogin" class="sso-button">
            <i class="nc-icon nc-key-25"></i>Login with Single Sign-On
          </button>
        </div>
        <div class="background-design">
          <div class="circle one"></div>
          <div class="circle two"></div>
          <div class="circle three"></div>
        </div>9
      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      handleSSOLogin() {
        // Add your Single Sign-On login logic here
        console.log('Single Sign-On login clicked');
      },
    },
  };
  </script>
  
  <style scoped>
  /* Container */
  .login-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 100vh;
    overflow: hidden;
  }
  
  /* Left Panel with Background Image */
  .left-panel {
    background: url("https://img.lovepik.com/photo/45009/7677.jpg_wh860.jpg") no-repeat center center;
    background-size: contain;
  }
  
  
  /* Right Panel with Dark Blue Background */
  .right-panel {
    background-color: #3a21f6;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }
  
  /* Login Card */
  .logo {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .login-card {
    background: rgba(255, 255, 255, 0.9);
    padding: 40px 30px;
    border-radius: 15px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    text-align: center;
    z-index: 10;
    position: relative;
  }
  
  /* Logo */
  .logo img {
    width: 120px;
    margin-bottom: 20px;
  }
  
  /* Welcome Text */
  h1 {
    margin-bottom: 10px;
    font-size: 24px;
    color: rgb(13, 13, 13);
  }
  
  .subtitle {
    font-size: 16px;
    color: #0e0d0d;
    margin-bottom: 30px;
  }
  
  /* SSO Button */
  .sso-button {
    background-color:#2a0ff5;
    color: #e9ebec;
    border: none;
    padding: 12px 20px;
    border-radius: 25px;
    cursor: pointer;
    font-size: 16px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background-color 0.3s ease;
    width: 100%;
    margin-bottom: 20px;
  }
  
  .sso-button i {
    margin-right: 8px;
  }
  
  .sso-button:hover {
    background-color:#1c06c5;
  }
  
  /* Separator */
  .or-separator {
    margin: 20px 0;
    position: relative;
    font-size: 14px;
    color: #aaa;
  }
  
  .or-separator span {
    background: rgba(255, 255, 255, 0.9);
    padding: 0 10px;
    position: relative;
    z-index: 1;
  }
  
  .or-separator::before {
    content: "";
    width: 100%;
    height: 1px;
    background: #ddd;
    position: absolute;
    top: 50%;
    left: 0;
    transform: translateY(-50%);
  }
  
  /* Alternative Login */
  .alternative-login {
    background-color: #f8f9fa;
    color: #31708f;
    border: 1px solid #31708f;
    padding: 12px 20px;
    border-radius: 25px;
    cursor: pointer;
    font-size: 16px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: background-color 0.3s ease;
    width: 100%;
  }
  
  .alternative-login i {
    margin-right: 8px;
  }
  
  .alternative-login:hover {
    background-color: #e2e6ea;
  }
  
  /* Background Design on the Right Panel */
  .background-design .circle {
    position: absolute;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.2);
    z-index: 1;
  }
  
  .background-design .circle.one {
    width: 300px;
    height: 300px;
    bottom: -150px;
    left: -150px;
  }
  
  .background-design .circle.two {
    width: 200px;
    height: 200px;
    top: -100px;
    right: -100px;
  }
  
  .background-design .circle.three {
    width: 150px;
    height: 150px;
    bottom: 100px;
    right: 50px;
  }
  </style>
  *