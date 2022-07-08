<template xmlns="http://www.w3.org/1999/html">
  <div class="bg-primary">
    <main class="container py-5">
      <SocialLinks/>
      <AboutMe/>
      <education/>
      <PageViews/>
    </main>
  </div>
</template>

<script>

import Education from "@/components/Education";
import SocialLinks from "@/components/SocialLinks";
import AboutMe from "@/components/AboutMe";
import PageViews from "@/components/PageViews";

export default {
  name: 'HomeView',
  components: {PageViews, AboutMe, SocialLinks, Education}
}
</script>
