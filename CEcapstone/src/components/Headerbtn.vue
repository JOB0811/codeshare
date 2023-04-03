<template>
    <div class="header">
      <div class="toggle-button" @click="toggleMenu">
        <svg viewBox="0 0 100 80" width="30" height="30">
          <rect width="100" height="10"></rect>
          <rect y="30" width="100" height="10"></rect>
          <rect y="60" width="100" height="10"></rect>
        </svg>
      </div>
        <a class = "Hbtn">목포 지역관광</a>
      <nav>
        <ul>
          <li><a href="#">홈</a></li>
          <li><a href="#">지역 소개</a></li>
          <li><a href="#">문의</a></li>
        </ul>
      </nav>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        menuOpen: false
      };
    },
    methods: {
      toggleMenu() {
        this.menuOpen = !this.menuOpen;
      }
    }
  };
  </script>
  
  <style>
  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem;
    background-color: #f8f8f8;
    border-bottom: 1px solid #ccc;
  }
  
  nav ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
  }
  
  nav li {
    margin-right: 1rem;
  }
  
  nav a {
    color: #333;
    text-decoration: none;
    font-weight: bold;
    font-size: 1.1rem;
  }

  a {
    padding-left: 30px;
  }

  .Hbtn {
    font-family: 'Nanum Gothic', sans-serif;
  font-size: 1.1rem;
  color: #333;
  letter-spacing: 2px;
  line-height: 1.5;
  text-align: center;
  }

 
  </style>