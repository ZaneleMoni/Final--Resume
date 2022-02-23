<template>
  <div id="testimonials">
    <h1>Testimonials</h1>
    <section id="testimonial">

      <div class="card-group" v-if="testimonials">
  <div class="card" v-for="testimonial of testimonials"
          :key="testimonial.id">
    <img :src="testimonial.img" class="photo" alt="image"/>
    <div class="card-body">
      <h5 class="card-title">{{ testimonial.fname }} {{ testimonial.lname }}</h5>
      <p class="card-text">{{ testimonial.text }}</p>
      <p class="card-text"><small class="text-muted">{{ testimonial.status }}</small></p>
    </div>
  </div>
</div>

    </section>
  </div>
</template>

<script>
import App from "../App.vue";
export default {
  data() {
    return {
      testimonials: null,
    };
  },
  mounted() {
    fetch("https://portfolio-project-testimonial.herokuapp.com/testimonials")
      .then((response) => response.json())
      .then((data) => (this.testimonials = data))
      .catch((err) => console.log(err.message));
    console.log(testimonials);
  },
  name: "testimonials",
  components: {
    App,
  },
};
</script>

<style scoped>
p {
  font-family: normal;
  font-size: 12px;
}


.row {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  flex-direction: row;
  margin: 2rem 0;
}
h1 {
  display: flex;
  margin-left: 30%;
  font-family: normal;
  padding: 81px;
}

  img {
  border-radius: 50%;
  margin: 15px auto 0;
  box-shadow: 0 8px 20px -4px #e02cd1;
  width: 100px;
  height: 100px;
}




@media screen and (min-width: 300px) {
  .card-img-top {
    flex-direction: column;
  }
  .card {
    display: flex;
  }
}
</style>
