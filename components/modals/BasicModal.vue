<template>
    <div class="basic-modal">
      <div class="content-modal">
        <div class="header">
          <h1>PODGLĄD</h1>
          <span @click="closeModal">Zamknij</span>
        </div>
        <div class="content">
          <slot></slot>
        </div>
  
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "BasicModal",
    methods: {
      closeModal() {
        const data = {
          state: false,
          content: null
        }
        this.$nuxt.$emit('closeModal', data);
      }
    }
  }
  </script>
  
  <style scoped>

  .basic-modal {
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    background-color: rgba(0,0,0, 0.5);
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
  }
  .basic-modal > .content-modal {
    display: inherit;
    flex-direction: column;
    width: 65%;
    height: 75%;
    background-color: #cae5ff;
    border-radius: 25px;
    padding: 20px;
  }
  .basic-modal > .content-modal > .header {
    display: flex;
    margin-top: 10px;
    margin-bottom: 20px;
    justify-content: space-between;
    width: 70%;
    margin-left: auto;
    margin-right: auto;
    max-height: 50px;
  }
  .basic-modal > .content-modal > .content {
    margin-left: auto;
    margin-right: auto;
    max-height: 90%;
  }
  span {
    cursor: pointer;
    font-size: x-large;
    color: black;
  }
  </style>