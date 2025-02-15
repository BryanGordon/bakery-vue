<script setup>
  import Logo from '../assets/logo.jpg'
</script>

<template>

  <header id="inicio">
    <picture>
      <img :src=Logo alt="logo-image">
    </picture>

    <div>
      <h4>Bakery</h4>
      <span>Tus postres de manera sencilla</span>
    </div>
  </header>

</template>

<style scoped>
  header {
    background-color: #0D0D0D;
    padding-block: 32px;
    display: flex;
    flex-direction: column;
  }

  picture {
    margin: 0 auto;
  }

  img {
    border-radius: 20px;
    max-width: 100px;
  }

  div {
    margin-left: 20px;
  }

  h4 {
    margin: 0 0 5px 0;
  }
</style>