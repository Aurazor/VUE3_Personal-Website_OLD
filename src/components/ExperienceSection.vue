<template>
  <section class="experience">
    <div class="experience-wrapper app-container">
      <div class="experience-text">
        <div class="experience-text-title">My Experience</div>
      </div>
      <div class="experience-timeline-cards">
        <TimelineCard icon="timeline-card-icon" year="2012" header="Sir Leckraz Teelock SSS" subtitle="At Sir Leckraz Teelock, I was captivated by the wonders of computer studies and mathematics. Algorithms, data structures, and programming as a whole had me under their spell, and I couldn't get enough of them. My focus was unwavering, and I couldn't wait to delve deeper into the exciting world of technology."/>
        <TimelineCard year="2019" header="University Of Technology Mauritius" subtitle="At the University of Technology Mauritius, I embarked on a thrilling journey in computer science, tackling coursework with a passion and unleashing my creativity in various projects. From building innovative web applications for the campus, to crafting immersive video games with Javascript, and developing sleek android applications with Java - I honed my computer skills and broadened my knowledge in the field like never before."/>
        <TimelineCard year="2022" header="Publicis Groupe" subtitle="At Publicis Groupe, I was part of a dynamic team working on the Mavieencouleurs.fr website where I contributed my expertise to the backend and mobile app development. My journey didn't stop there, as I was then challenged with a more complex project at Razorfish, where I showcased my skills in backend development using Java Quarkus and AWS. It was a thrilling experience that allowed me to expand my knowledge and grow as a professional."/>
      </div>
<!--      <div class="experience-timeline">-->
<!--        <img class="experience-timeline__image" src="../assets/images/diploma3d.png" alt="man with diploma">-->
<!--      </div>-->
    </div>
  </section>
</template>

<script>
import TimelineCard from "@/components/TimelineCard";

export default {
  name: "ExperienceSection",
  components:{
    TimelineCard
  }
}
</script>

<style lang="scss" scoped>
  .experience{
    .experience-wrapper{
      width: var(--container-width);
      height: 100%;
      padding: 15px 0;

      .experience-text{
        .experience-text-title{
          font-size: 1.5rem;
          margin-bottom: 30px;
        }

        .experience-text-subtitle{

        }
      }

      .experience-timeline-cards{
        padding: 0 25px;
      }

    }



  }
</style>