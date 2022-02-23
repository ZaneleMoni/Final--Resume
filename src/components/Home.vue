
<template>
<section id="home">
  <div id="content" class="pt-5 text-center">
    <h6 class=" display-6 fw-bold">HELLO! i am</h6 >
        <h1 class="display-4 fw-bold">Ntombizanele Moni</h1>

    <div class="col-lg-6 mx-auto">
      <p class="lead mb-4">Aspiring Software Developer.</p>
      <div class=" justify-content-sm-center mb-5 d-grid gap-4 d-flex">
              <a target="_blank" href="https://github.com/ZaneleMoni"><i class="fa fa-github"></i></a>

       <a target="_blank" href="https://www.linkedin.com/in/zanele-moni-b88559184/"><i class="fa fa-linkedin"></i></a> 
      </div>
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


h6,h1,p{
  color:aliceblue;
  font-family: 'Times New Roman', Times, serif;
}
#home{ 
  padding: 120px;
  height: 100vh;
   background-image: url('https://www.wallpapersun.com/wp-content/uploads/2021/10/windows-11-wallpaper-4k.jpg');
}

.hero{
    height: 100%;
    width: 100%;
    text-align: center;
    padding:  171px;
    /* margin-left: 180px; */
}
#name{
  padding: 71px;
  font-size: 50px;
  text-align:left;
  font-family: normal;
  color: black;

  
}
@media screen and (min-width:346px){
  
}

.typing-demo {
  width: 36ch;
  animation: typing 2s steps(30), blink 0.5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: monospace;
  font-size: 1.3em;
}

@keyframes typing {
  from {
    width: 100px;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
</style>

