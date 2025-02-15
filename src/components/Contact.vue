<script setup>
  import Facebook from '../icons/Facebook.vue';
  import Instagram from '../icons/Instagram.vue';
  import Whatsapp from '../icons/Whatsapp.vue';
</script>

<template>
  <section>
    <header>
      <h3>Contactos</h3>
    </header>

    <article>

      <div>
        <h4>Dirección</h4>
        <iframe
          title='ubicacion-local'
          src='https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3989.813144473951!2d-78.43586008528415!3d-0.09228959993264801!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x91d58f1f6a132d5b%3A0x2c50a94a08166d1a!2sCapit%C3%A1n%20Giovanni%20Calles%2C%20Quito!5e0!3m2!1ses!2sec!4v1637601695933!5m2!1ses!2sec'
          loading='lazy'
        />
      </div>

      <div>
        <h4>Teléfono</h4>
        <span>09931991</span>
      </div>

      <div>
        <h4>Redes sociales</h4>
        <Facebook />
        <Instagram />
        <Whatsapp />
      </div>
    </article>

  </section>
</template>

<style scoped>
  section {
    width: 75%;
    margin: 0 auto;
    margin-bottom: 30px;
  }

  h3 {
    font-size: 24px;
    margin: 24px 0 30px 0;
  }
 </style>