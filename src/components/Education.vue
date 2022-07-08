<template>
  <section>
    <div class="education py-3">
      <div class="row">
        <div class="col-6">
          <div class="d-flex align-items-center schoolColor">
            <i class="fa fa-university fa-2x ms-4" aria-hidden="true"></i>
            <h2 class="m-3 p-2 fst-italic fs-2"> Educations </h2>
          </div>
          <div class="m-2 fst-italic" v-for="item in education">
            <h4 class="my-2">{{ item.title }}</h4>
            <div class="d-flex align-items-center ">
              <h6 class="mb-2"> {{ item.date }} </h6>
            </div>
            <p>{{ item.paragraph }}</p>
          </div>
        </div>
        <div class="col-3">
          <div>
            <h2 class="fw-bold schoolColor fst-italic">
              Gained Skills
            </h2>
            <div>
              <div v-for="skill in skills">
                <h6 class="fst-italic grey-color">{{ skill }}</h6>
              </div>
            </div>
          </div>
        </div>
        <div class="col-3">
          <h2 class="fw-bold schoolColor fst-italic">
            Hobbies
          </h2>
          <div>
            <div v-for="hobbies in hobbies">
              <h6 class="fst-italic grey-color">{{ hobbies }}</h6>
            </div>
          </div>
        </div>
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
          date: ' Oct, 2020 - Present',
          paragraph: 'During this period I was learning how to do things right. ' +
              'Most of the time I was doing School Projects and listening to subjects ' +
              'that gonna teach me skills I didn\'t know before. I learned about design patterns, ' +
              'writting OOP code, MVC, SQL, NoSQL, project planning, database designing, etc.'
        },
        {
          title: 'High School(Economic–law–commercial department) Ljupco Santov - Kocani',
          date: 'Sept, 2016 - Jun,2020 ',
          paragraph: 'I finished my high school at "Ljupco Santov"-Kocani and gained knowledge in economics,\n' +
              '          law and trade, from here I can say for myself that I have acquired communication skills, team\n' +
              '          spirit, adaptability, leadership ...'
        }
      ],
      skills: ['HTML5', 'CSS3', 'Bootstrap', 'Javascript', 'Vue.js', 'C', 'C++', 'Git', 'Java'],
      hobbies:['Fashion','Design','Cooding','Gym','Reading Books','Skiing', 'Traveling'],
    }
  },
}
</script>

<style scoped>
.schoolColor {
  color: chocolate;
}
</style>