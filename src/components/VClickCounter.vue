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
    min-width: 300px;
    height: 200px;
    font-size: 160px;
    padding: 25px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 8px solid #fff017c4;
    margin: 15px;
  }
    .counter-button {
    width: 250px;
    height: 80px;
    font-family: Roboto, sans-serif;
    font-weight: bold;
    font-size: 35px;
    color: white;
    border: 2px solid white;
    border-radius: 15px;
    margin: 5px;
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
