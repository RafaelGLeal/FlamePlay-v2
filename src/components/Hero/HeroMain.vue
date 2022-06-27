<template>
  <div class="hero">
    <div class="hero-col-1">
      <div class="dot-image">
        <img src="@/assets/dotGrid.svg" alt="Dot grid image" />
      </div>
      <div class="hero-col-1__wrapper">
        <h2>O melhor bot multiuso do mundo ao seu alcance.</h2>
        <div class="btn-wrapper">
          <BtnSecondary btnAction="Comandos" />
          <BtnPrimary btnAction="Convidar bot" />
        </div>
      </div>
    </div>
    <div class="hero-col-2">
      <div class="hero-col-2__bg">
        <img src="@/assets/hero-bg-1.svg" alt="" />
        <div class="bg-noteIcon-1">
          <img src="@/assets/note-icon-1.svg" alt="" />
        </div>
        <div class="bg-noteIcon-2">
          <img src="@/assets/note-icon-2.svg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BtnPrimary from "@/components/Buttons/BtnPrimary.vue";
import BtnSecondary from "@/components/Buttons/BtnSecondary.vue";
export default {
  name: "HeroMain",
  components: { BtnPrimary, BtnSecondary },
};
</script>

<style lang="scss" scoped>
.hero {
  display: grid;
  grid-template-columns: 2fr 1fr;
  height: 80vh;
  margin-top: 5vh;
  &-col-1 {
    width: 100%;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .dot-image {
      position: absolute;
      top: 25%;
      left: 0;
    }
    h2 {
      margin-bottom: 2em;
    }
    .btn-wrapper {
      display: flex;
      gap: 2em;
    }
  }
  &-col-2 {
    width: 100%;
    &__bg {
      position: relative;
      z-index: 1;
      margin-top: 3em;
      img {
        max-width: 90%;
      }
      &::before {
        content: "";
        background-color: var(--c-blue);
        position: absolute;
        width: 70%;
        height: 100%;
        z-index: -1;
        right: 0;
        top: 5%;
        border-top-left-radius: 5em;
        border-bottom-left-radius: 5em;
      }
      .bg-noteIcon-1,
      .bg-noteIcon-2 {
        position: absolute;
      }
      .bg-noteIcon-1 {
        top: 0;
        left: -20%;
      }
      .bg-noteIcon-2 {
        bottom: 0;
        left: -20%;
      }
    }
  }
}
h2 {
  font-size: var(--fsize-lg);
  max-width: 18ch;
}
</style>
