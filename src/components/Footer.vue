<template>
  <section class="bg-dark border-bottom border-top border-warning border-5">
    <div class="footer container pt-5 pb-4">
      <div class="row">
        <div
            class="col-sm-12 col-md-4 col-lg-4 col-xl-4 d-flex align-items-center justify-content-center text-center flex-column">
          <br/>
          <h4 class="mb-2 fs-2 fw-bold text-secondary fontPara"> CV </h4>
          <p class="text-white fontPara"> If you like it give me a thumbs up for my CV I would be grateful:</p>
          <PageViews/>
        </div>
        <div class="col-12 col-md-4 col-lg-4 col-xl-4">
          <div class="border-end border-start border-warning border-4 px-5 my-5 fw-bold text-secondary fontPara">
            <h4 class="mb-2 fs-2 fw-bold ">Social Links</h4>
            <div v-for="item in apps" class="d-flex align-items-center mb-2 ">
              <a class="text-secondary" :href="item.link">
                <i class="fa me-3 text-white" :class="item.icon"></i>
                {{ item.name }}
              </a>
            </div>
            <br>
          </div>
        </div>
        <div class="col-12  col-md-4 col-lg-4 col-xl-4 my-4">
          <h4 class="my-3 fs-2 fw-bold text-secondary fontPara">Contact:</h4>
          <div class="text-white fontPara" v-for="item in social">
            <ul class="mb-1">
              <li class="mb-1 fs-5">{{ item }}</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

import PageViews from "@/components/PageViews";

export default {
  name: "Footer",
  components: {PageViews},
  data() {
    return {
      social: [
        'E-mail: anazaharijeva@gmail.com ',
        'Address: Goce Delcev 51 Kocani - North Macedonia',
        '+389 77 839 880',

      ],
      apps: [
        {
          name: 'GitHub',
          link: 'https://github.com/anazaharijeva',
          icon: 'fa-github fa-2x'
        },
        {
          name: 'LinkedIn',
          link: 'https://www.linkedin.com/in/ana-zaharijeva-558b32236',
          icon: 'fa-linkedin fa-2x'
        },
        {
          name: 'Instagram ',
          link: 'https://www.instagram.com/anazaharijeva/',
          icon: 'fa-instagram fa-2x'
        },
      ]
    }
  }
}
</script>

<style scoped>
.fontPara {
  font-family: Consolas;
}

</style>