<template>
  <section>
    <div class="AboutMe py-3">
      <div class="row">
        <div class="col-6 col-md-6 ">
          <div class="d-flex align-items-center schoolColor">
            <i class="fa fa-user-circle-o fa-2x  m-3 p-2" aria-hidden="true"></i>
            <h2 class="fst-italic fs-2"> About Me</h2>
          </div>
          <div class="fst-italic">
            <p> Hello, my name is Ana and I am student at 2nd year at the Faculty of Information
              Sciences and Computer Engineering - Ss. Cyril and Methodius University in Skopje.
              As a person I am open to new ideas and always motivated to learn something new.When I do something for the
              first time I invest fully and try to do it right, by nature I am curious and always ready to learn
              something new.
            </p>
          </div>
        </div>
        <div class="col-6 col-md-6 ">
          <div class="d-flex align-items-center schoolColor">
            <h4 class="m-3 p-2 fst-italic fs-2"> Languages</h4>
            <i class="fa fa-language fa-2x" aria-hidden="true"></i>
          </div>
          <div v-for="progress in languages" class="mb-3">
            <h6 class="fst-italic fw-bold">{{ progress.name }} </h6>
            <div class="progress">
              <div class="progress-bar progress-bar-striped bg-warning" role="progressbar"
                   :style="{width: progress.progressWidth}"
                   aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">
                <div class="fw-bold">{{ progress.language }}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutMe",
  data() {
    return {
      languages: [
        {
          name: 'Macedonian language',
          language: 'Native',
          progressWidth: '100%',
        },
        {
          name: 'English language',
          language: 'Fluent',
          progressWidth: '80%'
        }
      ]
    }
  }
}
</script>

<style scoped>
.schoolColor {
  color: chocolate;
}
</style>