<template>
  <!-- ======= About Section ======= -->
  <section id="both">
    <section id="about" class="about">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>About</h2>
        </div>

        <div class="row">
          <div class="col-lg-4">
            <img src="https://i.postimg.cc/Kjt2QpKG/zanele2.jpg" class="img-fluid" alt="">
          </div>
          <div class="col-lg-8 pt-4 pt-lg-0 content">
            <h3>Aspiring Software Developer</h3>
            
            <div class="row">
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-rounded-right"></i> <strong>Birthday:</strong> 25 Dec 1997</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>LinkedIn:</strong> Zanele Moni</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>Phone:</strong> +27 62 433 4358</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>City:</strong> City : Western Cape, CAPE TOWN</li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul>
                  <li><i class="bi bi-rounded-right"></i> <strong>Age:</strong> 24</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>Highest Grade:</strong> Grade 12</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>Email:</strong> zanelemmoni4@gmail.com</li>
                  <li><i class="bi bi-rounded-right"></i> <strong>Freelance:</strong> Available</li>
                </ul>
              </div>
            </div>
            <p>
    My communication and organizational skills <br>are exceptional, as well as my
      ability to work under pressure even in times of change,I'm keen to develop
      a new skill and use existing skills to perform a variety of tasks
      successfully,If given an opportunity I believe that I can be a great asset
      to any team.
            </p>
          </div>
        </div>

      </div>
    </section><!-- End About Section -->

    <!-- ======= Skills Section ======= -->
    <section id="skills" class="skills">
      <div class="container" data-aos="fade-up">

        <div class="section-title">
          <h2>Skills</h2>
        </div>

        <div class="row skills-content">

          <div class="col-lg-6">

            <div class="progress">
              <span class="skill">HTML <i class="val">100%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 100%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

            <div class="progress">
              <span class="skill">CSS <i class="val">90%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 90%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

            <div class="progress">
              <span class="skill">JavaScript <i class="val">75%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 75%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

          </div>

          <div class="col-lg-6">

            <div class="progress">
              <span class="skill">Bootstrap <i class="val">80%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 80%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

            <div class="progress">
              <span class="skill">MySQL <i class="val">90%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 90%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

            <div class="progress">
              <span class="skill">Node J.S<i class="val">55%</i></span>
              <div class="progress-bar-wrap">
  <div class="progress-bar bg-success" role="progressbar" style="width: 55%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>              </div>
            </div>

          </div>

        </div>

      </div>
    </section><!-- End Skills Section -->
</section>
</template>

<script>
export default {

}
</script>

<style>
/*--------------------------------------------------------------
# About
--------------------------------------------------------------*/
#about{
  padding: 71px;
}
h2{
  font-size: 40px;
}
.about .content h3 {
  font-weight: 700;
  font-size: 26px;
  color: #555555;
}
.about .content ul {
  list-style: none;
  padding: 0;
}
.about .content ul li {
  padding-bottom: 10px;
}
.about .content ul i {
  font-size: 20px;
  padding-right: 2px;
  color: #34b7a7;
}
.about .content p:last-child {
  margin-bottom: 0;
}

/*--------------------------------------------------------------
# Skills
--------------------------------------------------------------*/
.skills .progress {
  height: 60px;
  display: block;
  background: none;
  border-radius: 0;
}
.skills .progress .skill {
  padding: 10px 0;
  margin: 0 0 6px 0;
  text-transform: uppercase;
  display: block;
  font-weight: 600;
  font-family: "Poppins", sans-serif;
  color: #222222;
}
.skills .progress .skill .val {
  float: right;
  font-style: normal;
}
.skills .progress-bar-wrap {
  background: #f3f3f3;
}
.skills .progress-bar {
  width: 1px;
  height: 10px;
  transition: 0.9s;
  background-color: #34b7a7;
}
</style>