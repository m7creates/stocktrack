<script setup>
import { RouterLink, RouterView } from 'vue-router'
import logo from './assets/logo.png'
</script>

<template>
  <header>
    <figure>
      <a href="/"><img :src="logo" alt="site universal logo"></a>      
    </figure>
    <p class="main-header">Out of Stock records</p>

  </header>

  <RouterView />

  <footer>
    <figure>
      <a href="/"><img :src="logo" alt="site universal logo"></a>      
    </figure>
    <div>
      <RouterLink to="/about">About Us</RouterLink>
      <RouterLink to="/articles">Articles</RouterLink>
      <RouterLink to="contact">Contact Us</RouterLink>
    </div>
  </footer>
</template>

<style scoped>
  header{
    padding-top: 2rem; padding-left: .64rem;
    display: flex;
    gap: 1rem;
    align-items: center;

    border-bottom: 1px solid;
  }

  header p{
    color: var(--primary-color);
  }

  img{
    height: 2rem;
  }

  nav{
    display: flex;
    gap: .8rem;
  }

  nav a{
    text-decoration: none;
  }

  footer{
    border-top: 1px solid var(--primary-color);
    display: flex; gap: 1.2rem; align-items: center;
  }
  footer div{
    display: flex; gap: .8rem;
  }
   footer a{
    text-decoration: none;
    color: var(--primary-color);
   }


</style>
