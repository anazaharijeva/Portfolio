<template xmlns="http://www.w3.org/1999/html">
  <main class="bg-primary">
    <SocialLinks/>
    <div class="container py-5">
      <AboutMe/>
      <education/>
    </div>
    <Footer/>
  </main>
</template>

<script>

import Education from "@/components/Education";
import SocialLinks from "@/components/SocialLinks";
import AboutMe from "@/components/AboutMe";
import Footer from "@/components/Footer";

export default {
  name: 'HomeView',
  components: {Footer, AboutMe, SocialLinks, Education}
}
</script>
