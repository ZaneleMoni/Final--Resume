<template>
<section class="container">
 <title>My Skills Section</title>
   <div class="skills-section">
    <div class="skills-header">
     <h1>Skills</h1>   
     </div>
     <div class="skills-container">
       
      <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://cdn.freebiesupply.com/logos/large/2x/html-5-logo-png-transparent.png"     alt="" class="skills-icons">
        </div>
         <h3>HTML 5</h3>
        </div>
       </div>
       
       
        <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/CSS.3.svg" alt="" class="skills-icons">
        </div>
        <h3>CSS3</h3>
        </div> 
       </div>
       
       
        <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="hhttps://www.pngitem.com/pimgs/m/171-1718042_javascript-logo-png-transparent-png.png" alt="JavaScript image" class="skills-icons">
        </div>
        <h3>JAVASCRIPT</h3>
        </div>
       </div>
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="http://pluspng.com/img-png/nodejs-logo-png-nice-images-collection-node-js-desktop-wallpapers-370.png" alt="Node.js immage" class="skills-icons">
        </div>
        <h3>NODE.JS</h3>
        </div>
       </div>
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://miro.medium.com/max/1024/1*9HanDsRU11ZMsgDGJwN96w.png" alt="Bootstrap image" class="skills-icons">
        </div>
        <h3>BOOTSTRAP</h3>
        </div>
       </div>
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSHZqKnJISAUbxRIBKW51Nd0sTsfMbuBsC-A2gWKhUpxdUDTQ4faiwg9Ne22EDes_PuMq8&usqp=CAU" alt="" class="skills-icons">
        </div>
        <h3>MySQL</h3>
        </div>
       </div>
       
       
       </div>
    
     </div>
   
    </section>
</template>

<script>
export default {};
</script>

<style scoped>


*{
padding: 0;
margin: 0;
box-sizing: border-box;
font-family: Arial, sans-serif;
}

body{
background: #ccc;
}

.skills-section{
padding-top: 20px;
}

.skills-header{
text-align: center;
color: #fff;
padding: 1rem;
position: relative;
}

.skills-header:after{
content: '';
position: absolute;
bottom: 0;
left: 50%;
transform: translateX(-50%);
width: 100px;
height: 4px;
background-color: #2ecc71;
border-radius: 2px;
}

.skills-container{
display: grid;
grid-tempLate-columns: repeat(5, 1fr);
justify-content:center;
align-items:center;
text-align: center;
grid-gap:1rem;
padding: 1rem 80px;
font-size: 1.2rem;
}
.skills-box{
padding: 1rem;
color: #000;
cursor:pointer;
}
/* .skills-box:hover > .skills-title: after
.skills-box:hover > .skills-title: before{
 width: 30px;
} */
.skills-box:hover .skills-img{
transform: translateX(-20px);
}

.skills-title{
display:flex;
flex-direction: column;
align-items:center;
padding: 0.5rem;
margin-bottom: 0.5rem;
position: relative;
}

.skills-title:after{
content: '';
position:absolute;
bottom: 0;
right: 50%;
width:20px;
height:4px;
border-radius: 2px 0 0 2px;
background-color: #2ecc71;
transition: .5s;
}

.skills-title:before{
content: '';
position:absolute;
bottom: 0;
left: 50%;
width:100px;
height:4px;
border-radius: 0 2px 2px 0;
background-color: #2ecc71;
}

.skills-icons{
width:50px;
z-index:2;
}

.skills-img{
width:90px;
height:90px;
position: relative;
border-radius: 45px;
background-color: #fff;
display:flex;
justify-content:center;
align-items:center;
transition: .5s;
}

.skills-img:after{
content: '';
position:absolute;
top:0;
left: 0;
width:50%;
height:90px;
background: rgba(100, 100, 100, 0.5);
border-radius: 45px 0 0 45px;
}
.skills-title h3{
color: #333;
margin-top: 0.5rem;
}
@media screen and (max-width:990px){
 .skills-container{
 grid-tempLate-columns: repeat(2, 1fr);
 padding: 2rem 50px;
 }
}

@media screen and (max-width:650px){
 .skills-container{
 grid-tempLate-columns:2fr;
 padding: 2rem 50px;
 }
}
</style>
