
<template>

  
<section class="hero p-5" id="hero">
  <div class="hero-container">
    <div class="hero-content">
      <h1 class="hero-header">
         Ntombizanele Moni
        </h1>
      <h2 class="hero-subheader">
        Full Stack Developer </h2>
      <div class="try-business">
        <a href="#about" >Read More</a>
        
      </div>
    </div>
  </div>
  <div class="col-lg-6 mx-auto">
      <div class=" justify-content-sm-center mb-5 d-grid gap-4 d-flex">
              <a target="_blank" href="https://github.com/ZaneleMoni"><i class="fa fa-github"></i></a>

       <a target="_blank" href="https://www.linkedin.com/in/zanele-moni-b88559184/"><i class="fa fa-linkedin"></i></a> 
      </div>
    </div>
</section>
    
 
</template>

<script>
export default {
name:"hero",
components:{
},
data() {
    return {
        
    }
},
}
</script>

<style scoped>


body {
  font-family: "Open Sans", sans-serif;
  color: rgb(71, 82, 93);
}
.hero {
  background-color: rgb(227, 238, 252);
  background-image: url("https://cfl.dropboxstatic.com/static/images/business/homepage/background--db-vfl4SbjZf.jpg");
  background-repeat: no-repeat;
  background-position: right center;
}
.hero-container {
  min-height: 500px;
  padding: 75px 20px;
  max-width: 990px;
  margin: 0 auto;
  position: relative;
}
.hero-content {
  max-width: 450px;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}
.hero-header, .hero-subheader {
  font-weight: 300;
}
.hero-header {
  font-size: 47.25px;
  margin-bottom: 20px;
}
.hero-subheader {
  font-size: 21px;
  padding-bottom: 20px;
  margin-bottom: 0;
}
.try-business {
  margin: 30px 0 0 0;  
}
.try-business-button {
  display: inline-block;
  border-radius: 5px;
  font-size: 21px;
  text-decoration: none;
  padding: 19px 26px;
  color: #fff;
  background-color: rgb(0, 113, 224);
}
.try-business-button:hover {
  background-color: #3398ea;
}
.try-business-footer {
  display: block;
  font-size: 16px;
  margin-top: 15px;
}
.try-business-footer a {
  text-decoration: none;
  color: #0071e0;
  border-bottom: 1px solid #0071e0;
}
@media (max-width: 767px) {
  .hero {
    background-size: cover;
    background-position: 130px center;
  }
  .hero-container {
    min-height: 350px;
    padding: 45px 20px;
  }
  .hero-header {
    font-size: 31px;
    margin-bottom: 20px;
  }
  .hero-subheader {
    font-size: 16px;
  }
  .try-business-button {
    padding: 16px 40px;
    font-size: 16px;
  }
}
@media (max-width: 479px) {
  .hero {
    background-image: none;
  }
  .hero-content {
    right: 15px;
    left: 15px;
  }
  .hero-header {
    font-size: 26px;
  }
  .hero-header, .hero-subheader {
    text-align: center;
  }
  .try-business {
    text-align: center;
  }
}

</style>

