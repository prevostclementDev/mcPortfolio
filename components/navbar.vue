<script setup lang="ts">
</script>

<template>
  <header class="menu">
    <div class="logo">
      <NuxtLink to="/">
        <img src="~/public/logo.png"  alt="Logo de Maurine Callot"/>
      </NuxtLink>
    </div>
    <nav>
      <ul>
        <li><NuxtLink to="/">Hub</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/contact">Contact</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem 3.6rem;
  position: relative;
  z-index: 1;

  .logo {
    img {
      width: 108px;
      height: auto;
      object-fit: contain;

    }

  }

  nav {
    ul {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 3rem;

      a {
        color: #FFF;
        text-decoration: none;
        font-size: 22px;
        font-weight: 900;

      }

    }

  }

}
</style>