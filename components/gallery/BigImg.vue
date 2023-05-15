<template>
    <div v-if="image.length > 0">
        <img :src="image" class="img">
    </div>
  </template>
  
  <script>
  export default {
    name: 'BigImg',
    props: {
        image:{
            type: String,
            default: () =>''
        }
    }
  }
  </script>
  
  <style scoped>

  .img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding: 25px;
    width:30%;
    
  }

  @media (max-width: 650px){
    .img{
        display: block;
    }
  }
  </style>
  