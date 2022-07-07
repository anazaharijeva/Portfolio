<template>
  <section>
    <div class="education">
      <div class="d-flex align-items-center ">
        <i class="fa fa-university fa-2x ms-4" aria-hidden="true"></i>
        <h2 class="m-3 p-2"> Educations </h2>
      </div>
      <div class="m-2" v-for="item in education">
        <h4 class="my-2">{{item.title}}</h4>
        <div class="d-flex align-items-center ">
          <h6 class="mb-2"> {{item.date}} </h6>
          <i class="fa fa-spinner fa-spin mb-2" aria-hidden="true"></i>
        </div>
        <p>{{item.paragraph}}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Education",
  data() {
    return {
      education: [
        {
          title: 'Bachelor degree, Ss. Cyril and Methodius University in Skopje - In process',
          date:  ' Oct, 2020 - ',
          paragraph: 'I am a 2nd year student... for this time spent studying I can say that I have gained a great deal of\n' +
              '          knowledge in the field of informatics. I enrolled in this faculty because I have always loved Web Develop and\n' +
              '          Web Design where you can be creative.During my studies, I learned how to do things the right way. Most of the\n' +
              '          time I was doing school projects and listening to subjects that would teach me skills I didn\'t know. I learned\n' +
              '          about design patterns, writing OOP code, project planning, database design, structured programming, scripting\n' +
              '          and markup languages. I don\'t have any work experiences because I\'m still a student, but I can leave you a\n' +
              '          link from GitHub where you can see my projects made for the subject assignments in college'
        },
        {
          title: 'High School(Economic–law–commercial department) Ljupco Santov - Kocani',
          date: 'Sept, 2016 - Jun,2020 ',
          paragraph: 'I finished my high school at "Ljupco Santov"-Kocani and gained knowledge in economics,\n' +
              '          law and trade, from here I can say for myself that I have acquired communication skills, team\n' +
              '          spirit, adaptability, oratory skills for a wider audience, leadership ... . Also in this school we studied\n' +
              '          statistics, economic mathematics and studied C++ programming language for two years, so from here I have the\n' +
              '          basics.'
        },

      ]
    }
  }
}
</script>

<style scoped>

</style>