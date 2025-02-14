<script setup>
  import ProductsList from '../store/products.json'

  const products = ProductsList 
</script>

<template>
  <section>
    <header>
      <h3>Lista de postres</h3>
    </header>

    <article v-for="product in products">
      <picture>
        <img :src=product.image :alt=product.name_product>
      </picture>

      <div>
        <h4>{{ product.name_product }}</h4>
        <p>{{ product.product_description }}</p>
      </div>
    </article>
  </section>
</template>

<style scoped>
  section {
    width: 75%;
    color: wheat;
    margin: 0 auto;
  }

  h3 {
    font-size: 24px;
    margin: 24px 0 30px 0;
  }

  article {
    display: flex;
    justify-content: space-evenly;
  }

  img {
    max-width: 200px;
  }

  div {
    max-width: 75%;
  }
</style>