<template>
  <section>
    <div class="social-links">
      <div class="row">
        <div class="col-12 col-md-6 col-lg-4 col-xl-3">
          <img src="../assets/1.1.jpg" class="rounded-circle border border-warning border-4" alt="Profile image">
        </div>
        <div class="col-12 col-md-6 col-lg-4 col-xl-2">
          <div class="border-warning border-4 nameColor">
          <h4 class="my-2 mt-5 p-3 fw-bold"> Ana Zaharijeva</h4>
          <h5 class="p-4 fw-bold"> Web Develop</h5>
          </div>
        </div>
        <div class="col-12 col-md-6 col-lg-4 col-xl-3">
          <div class="border-end border-start border-warning border-4 px-5 my-5 fw-bold nameColor">
            <h4 class="mb-2 fs-2 fw-bold">Social Links</h4>
            <div v-for="item in apps" class="d-flex align-items-center mb-2 ">
              <a class="text-secondary" :href="item.link">
                <i class="fa me-3 text-black" :class="item.icon"></i>
                {{ item.name }}
              </a>
            </div>
            <br>
          </div>
        </div>
        <div class="col-12  col-md-6  col-lg-4 col-xl-3 my-4">
          <h4 class="my-3 fs-2 fw-bold nameColor">Contact:</h4>
          <div class="" v-for="item in social">
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
export default {
  name: "SocialLinks",
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
.nameColor{
  color: chocolate;
}
</style>