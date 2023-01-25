<script setup lang="ts">
  import { ref } from 'vue'

  const count = ref(0)
</script>

<template>
  <div>
    <div class="card">{{ count }}</div>
    <button type="button" class="counter-button click-button" @click="count++">Click</button>
    <button type="button" class="counter-button reset-button" @click="count=0">Reset</button>
  </div>
</template>

<style lang="scss" scoped>
  .card{
    width: 90vw;
    max-width: 500px;
    height: 200px;
    font-size: 10em;
    margin: 15px auto;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 8px solid #fff017c4;
  }
    .counter-button {
      width: 40%;
      max-width: 250px;
      min-width: 120px;
      height: 80px;
      font-family: Roboto, sans-serif;
      font-weight: bold;
      font-size: 35px;
      color: white;
      border: 2px solid white;
      border-radius: 15px;
      margin: 5px 15px;
      cursor: pointer;
    }

    .counter-button:hover {
      background-color: #00471b;
    }

    .click-button {
      background-color: #41B883;
    }

    .reset-button {
      background-color: #bd34fe;
    }
</style>
