<template>
  <main class="container">
    <div class="portfolio">
      <h3 class="my-2">  Ana Zaharijeva - CV </h3>
      <h6 class="my-2"> IT - Information Tehnologies </h6>
    </div>
    <SocialLinks/>
    <AboutMe/>
    <education/>
  </main>
</template>

<script>

import Education from "@/components/Education";
import SocialLinks from "@/components/SocialLinks";
import AboutMe from "@/components/AboutMe";

export default {
  name: 'HomeView',
  components: {AboutMe, SocialLinks, Education}
}
</script>
