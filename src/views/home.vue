<template>
  <div>
    <div class="hero">
      <img src="..\assets\resources\photos\header.jpg" alt="" srcset="" />
      <div
        class="column is-8-widescreen is-10-desktop is-full-touch "
        style="justify-content: start; margin: auto 0"
      >
        <h1
          class="has-text-warning is-size-1-desktop is-size-2-mobile is-size-1-tablet is-family-primary"
        >
          Bezalel Handyman Services
        </h1>
        <h4
          class="has-text-grey-darker	 subtitle is-size-4-mobile  is-size-2-tablet  is-family-secondary"
        >
          talent on loan from god, Exodus36:1
        </h4>
      </div>
    </div>
    <culture />
    <about-us />
    <skills />
    <contact />
  </div>
</template>
<script>
import culture from "@/components/culture";
import aboutUs from "@/components/about-us";
import skills from "@/components/skills";
import contact from "@/components/contact";
export default {
  name: "home",
  data() {
    return {
      modal: false
    };
  },
  components: {
    culture,
    aboutUs,
    skills,
    contact
  },
  methods: {}
};
</script>
<style scoped>
img {
  width: 100%;
  height: 100%;
  position: absolute;
  object-fit: cover;
  bottom: 0;
  right: 0;
  z-index: 1;
}
* {
  z-index: 3;
}
.hero {
  height: 100vh;
  position: relative;
}
.heroTitle {
  z-index: 2;
}
.notification {
  margin-bottom: 0;
}
</style>
