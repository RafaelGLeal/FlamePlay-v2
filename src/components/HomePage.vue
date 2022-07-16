<template>
  <HeroMain />
  <DetailsMain />
  <AboutMain/>
</template>

<script>
import HeroMain from "@/components/Home/HeroMain.vue";
import DetailsMain from "./Home/DetailsMain.vue";
import AboutMain from "./Home/AboutMain.vue";
export default {
  name: "HomePage",
  props: {
    msg: String,
  },
  components: { AboutMain, DetailsMain, HeroMain },
};
</script>
