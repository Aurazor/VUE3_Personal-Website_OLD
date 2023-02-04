<template>
  <section class="experience">
    <div class="experience-wrapper app-container">
     <h1 class="highlight-text">Education</h1>
      <div class="experience-timeline-cards">
        <TimelineCard year="2012" header="Sir Leckraz Teelock SSS" subtitle="subtitle"/>
        <TimelineCard year="2019" header="University Of Technology Mauritius" subtitle="subtitle"/>
        <TimelineCard year="2022" header="Publicis Groupe" subtitle="subtitle"/>
      </div>
<!--      <div class="experience-timeline">-->
<!--        <img class="experience-timeline__image" src="../assets/images/diploma3d.png" alt="man with diploma">-->
<!--      </div>-->
    </div>
  </section>
</template>

<script>
// import TimelineBox from "@/components/TimelineBox";
// import HeadingIcon from "@/components/HeadingIcon";
import TimelineCard from "@/components/TimelineCard";

export default {
  name: "ExperienceSection",
  components:{
    // HeadingIcon,
    TimelineCard
  }
}
</script>

<style lang="scss" scoped>
  .experience{
    background-color: #f8f8ff;
    .experience-wrapper{
      width: var(--container-width);
      height: 100%;
      padding: 50px 0;

      h1{
font-size: 2.1rem;
      }
      .experience-timeline-cards{
        padding: 0 25px;
        .timeline-card{
        }
      }

    }



  }
</style>