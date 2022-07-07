<template>
  <section>
    <div class="social-links">
      <div class="row">
        <div class="col-12 col-md-6  col-lg-4 col-xl-4">
          <img src="../assets/1.1.jpg">
        </div>
        <div class="col-12 col-md-6  col-lg-4 col-xl-4 ">
          <div class="m-5">
            <h4 class="mb-2">Social Links</h4>
            <div class="d-flex align-items-center mb-2">
              <i class="fa fa-github" aria-hidden="true"></i>
              <a class="text-decoration-none" href="https://github.com/anazaharijeva"> GitHub</a>
            </div>
            <div class="d-flex align-items-center mb-2">
              <i class="fa fa-trello" aria-hidden="true"></i>
              <a class="text-decoration-none" href="https://trello.com/b/UIm5kVd3/notes"> Trello</a>
            </div>
            <div class="d-flex align-items-center mb-2">
              <i class="fa fa-linkedin" aria-hidden="true"></i>
              <a class="text-decoration-none" href="https://www.linkedin.com/in/ana-zaharijeva-558b32236/"> LinkedIn</a>
            </div>
            <div class="d-flex align-items-center mb-2">
              <i class="fa fa-instagram" aria-hidden="true"></i>
              <a class="text-decoration-none" href="https://www.instagram.com/anazaharijeva/"> Instagram </a>
            </div>
            <br>
          </div>
        </div>
        <div class="col-12  col-md-6  col-lg-4 col-xl-4 my-4 ">
          <h4 class="my-3">Contact:</h4>
          <div v-for="item in social">
            <ul>
              <li>{{ item }}</li>
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
        'Address: Goce Delcev 51 ',
        'City: Kocani - North Macedonia',
        '+389 77 839 880',
        'Birthday: 20 November 2001',
        'Degree: in progress',
      ],
      links: [
        'GitHub',
        'Trello',
        'LinkedIn',
        'Instagram',
      ]
    }
  }
}
</script>

<style scoped>

</style>