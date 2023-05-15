<template>
    <div class="nav">
        <NuxtLink to='/' class="nav-item">Strona główna</NuxtLink>
      <NuxtLink to='/nasa' class="nav-item">Nasa</NuxtLink>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TopNav'
  }
  </script>
  
  <style scoped>
  .nav{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    background-color: #2891D7;
    min-height: 50px;
    box-shadow: 0px 5px 12px 0px #627988;
    border-bottom: 5px solid #86BDF1; 
    margin-bottom: 15px;
  }

  .nav-item{
    padding: 16px 5px 10px 5px;
    color: #d9ebfb;
    font-weight: bold;
    text-decoration: none;
    cursor: pointer;
  }

  .nav-item:hover {
    background-color: #86BDF1; 
    color: white;
  }

  </style>
  