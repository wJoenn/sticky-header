<template>
  <div>
    <header style="background-color: red; padding: 16px; position: sticky; top: 0; z-index: 10;">Hello world</header>
    <main>
      <p>aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa</p>
      <p
        v-for="n in 1000"
        :key="n"
        :data-aos="n % 2 ? 'fade-right' : 'fade-left'"
        style="padding: 32px; width: max-content; margin: 0 auto;"
      >
        {{ n }}
      </p>
    </main>
  </div>
</template>

<script setup>
  import 'aos/dist/aos.css';
  import AOS from 'aos';

  AOS.init()
</script>

<style>
  body {
    margin: 0;
    overflow-x: hidden;
  }
</style>
