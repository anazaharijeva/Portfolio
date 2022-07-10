<template>
  <section class="bg-dark border-bottom border-top border-warning border-5">
    <div class="social-links container p-4">
      <div class="row">
        <div class="col-12 col-md-6 col-lg-4 col-xl-4">
          <img src="../assets/1.1.jpg" class="rounded-circle border border-warning border-5 fontPara"
               alt="Profile image">
        </div>
        <div class="col-12 col-md-6 col-lg-4 col-xl-2">
          <div class="border-warning border-5">
            <h4 class="my-2 mt-5 p-3 fw-bold fs-3 text-secondary fontPara"> Ana Zaharijeva</h4>
            <h5 class="p-3 fw-bold fs-4 text-white fontPara"> Web Developer</h5>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SocialLinks",

}
</script>

<style scoped>
.fontPara {
  font-family: Consolas;
}

</style>