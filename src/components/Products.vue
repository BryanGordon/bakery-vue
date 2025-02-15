<script setup>
  import ProductsList from '../store/products.json'

  const products = ProductsList 
</script>

<template>
  <section>
    <header>
      <h3>Lista de postres</h3>
    </header>

    <article>
      <div class="container-products" v-for="product in products">
        
        <picture>
          <img :src=product.image :alt=product.name_product>
        </picture>

        <div class="product-info-container">
          <h4>{{ product.name_product }}</h4>
          <p>{{ product.product_description }}</p>
        </div>

      </div>
    </article>
  </section>
</template>

<style scoped>
  section {
    width: 75%;
    margin: 0 auto;
  }

  h3 {
    font-size: 24px;
    margin: 24px 0 30px 0;
  }

  .container-products {
    display: flex;
    justify-content: space-evenly;
    margin-bottom: 50px;
  }

  img {
    max-width: 200px;
    height: 150px;
    border-radius: 20px;
  }

  .product-info-container {
    max-width: 75%;
    margin-left: 30px;
  }

  @media screen and (width <= 950px) {
    .container-products {
      flex-direction: column;
    }

    .product-info-container {
      margin: 0;
    }
  }

</style>