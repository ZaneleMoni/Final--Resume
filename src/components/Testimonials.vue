<template>
<section id="">
<div id="testimonials" class="test p-5">
    <h1>Testimonials</h1>
  <div class="container mt-5 mb-5 p-5">
    <div class="row g-2">
        <div class="col-md">
        <div class="card-group1" v-if="testimonials">
     <div class="card p-3 text-center px-6" v-for="testimonial of testimonials"
          :key="testimonial.id">
   <div class="user-image"> <img :src="testimonial.img" class="rounded-circle" width="80"> </div>
       <div class="user-content">
         <h5 class="mb-8">{{ testimonial.fname }} {{ testimonial.lname }}</h5> <span>{{ testimonial.status }}</span>
                    <p>{{ testimonial.text }}</p>
                </div>
                <div class="ratings"> <i class="fa fa-star"></i> <i class="fa fa-star"></i> <i class="fa fa-star"></i> <i class="fa fa-star"></i> </div>
            </div>
        </div>
    </div>
</div>
  </div>
  </div>

</section>

  
</template>

<script>
import App from "../App.vue";
import testimonials from "../assets/js/testimonials"
export default {
  components:{
    testimonials
  },
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

.card-group1{
 gap:2rem;
 float:left;
	width:33.33333%;
 
    
}

.container{
  padding: 20px;
}

.card {
    border: none;   
}

.user-content p {
    margin-top: 5px;
    font-size: 12px
}

.ratings i {
    color: blue
}
</style>