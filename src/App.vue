<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <div class="foto">
    <img alt="Vue logo" class="logo" src="@/assets/IMG_20220824_072233-removebg-preview (1) (1).png" />
</div>

    <div class="wrapper">
      <HelloWorld msg="Indra Dheepa Bayu" />

      <nav>
        <RouterLink to="/">Profile</RouterLink>
        <RouterLink to="/skill">Skill</RouterLink>
        <RouterLink to="/portoView">Portofolio</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.foto{
  background-color: blue;
  border-radius: 50%;
  width: 175px;
  height: 175px;
  margin-right: 3rem;
  margin-left: -5rem;
}

img{
  border-radius: 50%;
  width: 175px;
  height: 175px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
