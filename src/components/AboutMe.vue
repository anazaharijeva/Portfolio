<template>
  <section>
    <div class="AboutMe">
      <div class="row">
        <div class="col-6">
          <div class="d-flex align-items-center m-3 p-2">
            <i class="fa fa-user-circle-o fa-2x" aria-hidden="true"></i>
            <h2> About Me</h2>
          </div>
          <p><span>Hello</span>, my name is Ana and I am a student on the Faculty of Information
            Sciences and Computer Engineering at Ss. Cyril and Methodius University in Skopje, Department of Information
            Technologies.
            As a person I am open to new ideas and always motivated to learn something new. I concentrate on making
            things
            better,
            not just bigger. When I do something for the first time I invest fully and try to do it right,
            by nature I am curious and always ready to learn something new.
          </p>
        </div>
        <div class="col-6">
          <h4 class="m-3 p-2"> Gained Skills </h4>
          <div class="progress">
            <div class="progress-bar progress-bar-striped" role="progressbar" style="width: 100%" aria-valuenow="100"
                 aria-valuemin="0" aria-valuemax="100">
              HTML
            </div>
          </div>
          <div class="progress">
            <div class="progress-bar progress-bar-striped bg-success" role="progressbar" style="width: 100%"
                 aria-valuenow="100" aria-valuemin="0" aria-valuemax="100">
              CSS
            </div>
          </div>
          <div class="progress">
            <div class="progress-bar progress-bar-striped bg-info" role="progressbar" style="width: 75%"
                 aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
              Java Script
            </div>
          </div>
          <div class="d-flex align-items-center ">
            <h4 class="m-3 p-2"> Languages</h4>
            <i class="fa fa-language fa-2x" aria-hidden="true"></i>
          </div>
          <div class="progress">
            <div class="progress-bar progress-bar-striped bg-warning" role="progressbar" style="width: 75%"
                 aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">English language
            </div>
          </div>
          <div class="progress">
            <div class="progress-bar progress-bar-striped bg-danger" role="progressbar" style="width: 100%"
                 aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"> Macedonian language
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutMe"
}
</script>

<style scoped>

</style>