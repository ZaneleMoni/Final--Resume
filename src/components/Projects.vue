<template>
  <section class="container">
    <div id="project">
      <h1>Projects</h1>
      <div class="card-group" v-if="projects">
        <div class="card" v-for="project of projects" :key="project.id">
          <img :src="project.img_url" class="photo" alt="image" />
          <div class="card-body">
            <h5 class="card-title">{{ project.title }}</h5>

            <div class="links justify-content-center">
              <a :href="project.github" class="card-link" target="_blank"
                ><i class="fa fa-github"></i></a
              ><br />
              <a :href="project.netlify" class="card-link" target="_blank"
                ><i class="fa fa-linkedin"></i
              ></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import App from "../App";
export default {
  data() {
    return {
      projects: [],
    };
  },

  mounted() {
    fetch("https://portfolio-project-testimonial.herokuapp.com/projects")
      .then((res) => res.json())
      .then((data) => (this.projects = data))
      .catch((err) => console.log(err.message));
  },
  name: "project",
  components: {
    App,
  },
};
</script>

<style scoped>
h1 {
  font-family: normal;
  display: flex;
  margin-left: 40%;
  padding: 50px;
  float:left;
	width:33.33333%;
}
img {
  align-content: center;
  gap: 3rem;
  height:180px;
  margin: 0 auto 1.5rem !important;
 
}
.card-group {
  text-align: center;
  gap: 2rem;
  width: 100%;
  height: 100%;
  padding: 2.5rem 2.5rem 1.5rem;
  
}
.links{
  display:flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}
</style>
