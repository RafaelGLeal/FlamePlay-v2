<template>
  <HeroMain />
  <DetailsMain />
</template>

<script>
import HeroMain from "@/components/Hero/HeroMain.vue";
import DetailsMain from "./Hero/DetailsMain.vue";
export default {
  name: "HomePage",
  props: {
    msg: String,
  },
  components: { DetailsMain, HeroMain },
};
</script>
