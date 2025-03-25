<script setup lang="ts">

</script>

<template>
  <footer>
    <img src="~/public/logo.png" alt="Logo de Maurine Callot">

    <ul class="socialMedia">
      <li><a href="https://www.linkedin.com/in/maurine-callot/">
        <img src="~/public/linkedin.svg" alt="">
      </a></li>
      <li><a href="https://www.instagram.com/maurine.callot/">
        <img src="~/public/instagram.svg" alt="">
      </a></li>
      <li><a href="https://www.facebook.com/maurine.callot/?_rdr">
        <img src="~/public/facebook.svg" alt="">
      </a></li>
    </ul>

    <div class="text">
      <p>Maurine Callot - Tous droits réservés</p>
      <NuxtLink to="/">Mentions légales</NuxtLink>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;

  & > img {
    width: 80px;
    height: 80px;
    object-fit: contain;

  }

  .socialMedia {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;

  }

  .text, a {
    color: white;
    text-decoration: none;
    font-size: 14px;
    text-align: center;
    margin: .6rem;
    display: block;

  }

}
</style>