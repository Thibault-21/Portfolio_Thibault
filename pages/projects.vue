<template>
  <div class="main">
      <div class="gallery">
        <div class="title">
          <h3>My statics and vue-projetcs </h3>
        </div>
        <div class="brick brick-1">
          <div class="image">
            <a rel="noreferrer"
               href="https://github.com/Thibault-21/Growthy" 
               target="_blank" 
               alt="Github_link">
                <img 
                  src="@/static/Images/marketplaceBtoB.png" 
                  alt="growthy project">
            </a>
          </div>
          <div class="details">
            <h4>Growthy</h4>
              <!-- descritpion -->
            <p> An app that I imagined to train myself </p>
              <!-- concept  -->
            <p><strong>Concept:</strong> BtoB Marketplace of fruits and vegetables</p>
              <!-- implementation -->
             <p>Implementation: 
              <strong>Vue.js, VueRouter, VueResource, Firebase</strong> and <strong>Vuex</strong>
             </p>
          </div>
        </div>
        <!--  -->
        <div class="brick brick-2">
          <div class="image">
            <a rel="noreferrer" 
               href="https://github.com/Thibault-21/DigitalWorkplace_surveyForm" 
               target="_blank" 
               alt="github link">
               <img src="@/static/Images/SurveyForm.png" 
                    alt="surveyForm project">
            </a>
          </div>
          <div class="details">
            <h4>SurveyForm</h4>
            <!-- descritpion -->
            <p>A small project that I imagined to learn <strong>Vue.js</strong></p>
            <!-- concept  -->
            <p><strong>Concept:</strong> A Survey about the digital workplace - 5 pages</p>
            <!-- implementation -->
            <p>Implementation: <strong> Vue.js</strong> </p>
          </div>
        </div>
        <!--  -->
        <div class="brick brick-3">
          <div class="details">
            <p><strong>Landing Page Projects</strong></p>
          </div>
        </div>      
        <!--  -->
        <div class="brick brick-4">
          <div class="image">
           <a rel="noreferrer"
              href="https://github.com/Thibault-21/Totem" 
              target="_blank" 
              alt="Github_link">
                <img class="totem" 
                     src="../static/Projects/Totem/Totem.png" 
                     alt="totem project">
           </a>
          </div>
          <div class="details">
            <h4>Totem </h4>
            <!-- descritpion -->
            <p>I imagined this project 6 months ago. 
            </p>
            <!-- concept  -->
             <p><strong>Concept:</strong>
             Coworking space in La Reunion (French Island).</p>
            <!-- implementation -->
            <p>Implementation: 
            <strong>HTML 5/CSS 3</strong></p>     
          </div>
        </div>
      </div>
    <nuxt />
  </div>

</template>


<style scoped>
.main {
  display: grid;
  height: 100%;
}

.gallery {
  display: grid; 
  grid-template-columns: 50% 50%;
  grid-template-rows: 5% 40% 40%;
  grid-gap: 20px;
  margin: 20px;
  height: 100%;
}
.title {
  grid-column-start: 1;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
  text-align: center;
  margin-bottom: 10px;
}
.brick {
  display: grid; 
  grid-template-columns: 60% 40%;
  grid-template-rows: 100%;
  grid-gap: 10px;

  background-color: rgba(211, 211, 211, 0.438); 
  border-radius: 5px;
  padding: 5px;
  margin: 5px;
  height: 100%;
}
.image {
  grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 1;
  grid-row-end: 2;
  height: 100%;
  transition: transform .1s;

}
.image:hover {
  transform: scale(1.4);

}
.details {
  padding: 5px;
}
img {
  height: 100%;
  width: 100%;
  border-radius: 5px;
}
.brick-1 {
  grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 2;
  grid-row-end: 3;
}
.brick-2 {
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 2;
  grid-row-end: 3;
}
.brick-3 {
  grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 3;
  grid-row-end: 4;
}
.brick-4 {
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 3;
  grid-row-end: 4;
}

video {
  border-radius: 5px;
  border: 10px solid white;

}
p {
  padding: 5px;
}
/* mobile phone */
@media only screen and (max-width: 768px) {
  h3 {
    font-size: 16px;
    text-align: center;
  }
  p, strong {
    padding-bottom: 10px;
    margin-bottom: 10px;
    margin-top: -10px;
  }
  .gallery {
    display: grid;
    grid-template-columns: 100%;
    grid-template-rows: 1% 30% 30% 0% 30%;
    margin: 10px;
    grid-gap: 30px; 
  }
  .brick {
    display: grid; 
    grid-template-columns: 100%;
    grid-template-rows: 50% 50%;
    grid-gap: 2px;

    background-color: rgba(211, 211, 211, 0.438); 
    border-radius: 5px;
    padding: 5px;
    margin: 5px;
  }
 
  .brick-1 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 2;
    grid-row-end: 3;
  }
  .brick-2 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 3;
    grid-row-end: 4;
  }
  .brick-3 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 4;
    grid-row-end: 5;
  }
  .brick-4 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 5;
    grid-row-end: 6;
    
  }
  img {
    height: 90%;
    width: 90%;
    border-radius: 5px;
  }
  .image {
    height: 100%;
  }
  .details {
  padding-bottom: 20px;
  margin-bottom: 10px
  }
}
</style>
