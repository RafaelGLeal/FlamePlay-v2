<template>
  <header>
    <div class="brand">
      <img src="@/assets/logo.svg" alt="Flame play logo" />
    </div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/commands">Commands</router-link>
      <BtnPrimary btnAction="Convidar Bot" />
    </nav>
  </header>

  <router-view />
</template>

<script>
import "@/style/reset.css";
import "@/style/normalize.css";
import "@/style/animations.css";
import "boxicons";
import BtnPrimary from "@/components/Buttons/BtnPrimary.vue";

export default {
  name: "App",
  components: {
    BtnPrimary,
  },
};
</script>

<style lang="scss">
:root {
  //colors
  --c-orange: #f26b1d;
  --c-orange-light: #fc6e1d;

  --c-white: #ffffff;
  --c-black-transparent: #26262633;
  --c-blue: #2f6073;
  --c-gray: #f2f2f2;
  --c-black: #262626;
  //font
  --f-brand: "Orbitron", sans-serif;
  --fweight-l: 500;
  --fweight-m: 600;
  --fweight-b: 700;
  --fsize-sm: 1em;
  --fsize-md: 1.5em;
  --fsize-lg: 2.5em;
}

body {
  box-sizing: border-box;
  background-color: var(--c-gray);
  font-size: 15px;
  font-family: "Open Sans", sans-serif;
  margin: 0 auto;
  max-width: 1440px;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2em 4em;
  nav {
    display: flex;
    align-items: center;

    a {
      margin: 0 1.5em;
      color: var(--c-black);
      font-weight: var(--fweight-l);
      padding: 0.5em;
      transition: 0.5s ease;
      border-radius: 0.5em;
      &:hover {
        background-color: var(--c-black-transparent);
        transition: 0.5s ease;
      }
    }
  }
}
</style>
