<template>
  <section class="border-bottom border-warning border-5">
    <div class="AboutMe py-3">
      <div class="row">
        <div class="col-12 col-md-6 ">
          <div class="d-flex align-items-center text-secondary">
            <i class="fa fa-user-circle-o fa-2x  m-3 p-2" aria-hidden="true"></i>
            <h2 class="fst-italic fs-2 mb-2"> About Me</h2>
          </div>
          <div class="fst-italic fs-5 my-2">
            <p> Hello, my name is Ana and I am student at the Faculty of Information
              Sciences and Computer Engineering - Ss. Cyril and Methodius University in Skopje -
              with never-stopping love for learning new tech. I am passionate about the Internet and how we can design
              beautiful looking interfaces with programming languages.
            </p>
          </div>
        </div>
        <div class="col-12 col-md-6 ">
          <div class="d-flex align-items-center text-secondary">
            <i class="fa fa-language fa-2x m-3 p-2" aria-hidden="true"></i>
            <h4 class="fst-italic fs-2 mb-2"> Languages</h4>
          </div>
          <div v-for="progress in languages" class="mb-3">
            <h6 class="fst-italic fw-bold">{{ progress.name }} </h6>
            <div class="progress">
              <div class="progress-bar progress-bar-striped progress-bar-animated bg-warning" role="progressbar"
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
        },
        {
          name: 'German language',
          language: 'Fluent',
          progressWidth: '50%'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>