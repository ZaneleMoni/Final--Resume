<template>
<div id="nav">
  <nav class="navbar navbar-dark bg-dark fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">NM</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="offcanvas offcanvas-end bg-dark" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
      <div class="offcanvas-header">
        <h5 class="offcanvas-title" id="offcanvasNavbarLabel">NM</h5>
        <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
      </div>
      <div class="offcanvas-body">
        <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#home"><i class=" 	fa fa-home"></i>Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about"> <i class=" 	fa fa-info-circle"></i>About</a>
          </li>
                <li class="nav-item">
            <a class="nav-link" href="#resume"><i class=" 	fa fa-mortar-board"></i>Resume</a>
          </li>
           <li class="nav-item">
            <a class="nav-link" href="#project"><i class=" fa fa-tasks"></i> Projects</a>
          </li>
           <li class="nav-item">
            <a class="nav-link" href="#testimonial"><i class=" fa fa-group"></i>Testimonials</a>
          </li>
           <li class="nav-item">
            <a class="nav-link" href="#contact"><i class=" 	fa fa-phone"></i>Contacts</a>
          </li>
        </ul>

      </div>
    </div>
  </div>
</nav>
</div>
</template>

<script>
export default {

}
</script>

<style>

</style>