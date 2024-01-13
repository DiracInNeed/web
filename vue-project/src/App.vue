<template>
  <div class="app">
      <h1>Hello World!</h1>
  </div>
  <people/>
</template>

<script lang="ts">
  import people from './components/people.vue';
  export default {
      name: 'App',
      components: { people }
  }
</script>

<style>
  .app {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100%;
      width: 100%;
      background-color: #98afde;
      border-radius: 5dvh;
      opacity: 0.8;
  }
</style>