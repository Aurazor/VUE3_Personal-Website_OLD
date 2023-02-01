<template>
  <section class="experience">
    <div class="experience-wrapper">
     <HeadingIcon heading="Experience"/>
      <div class="experience-timeline">
        <div class="experience-education experience-timeline-card-1">
          <TimelineBox class="white-timeline" year="2008" title="School" desc="I attended Nouvelle Decouverte Government School."/>
          <TimelineBox  year="2012" title="College" desc="For my secondary education I went to Sir Leckraz Teelock SSS."/>
          <TimelineBox  year="2019" title="University" desc="I went to University Of Technology Mauritius, where I took a course for Computer Science."/>
        </div>
        <div class="experience-professional experience-timeline-card-2">
          <TimelineBox class="white-timeline" year="2022" title="Mavieencouleurs.fr" desc="I worked on the Backend and Mobile aspect of the website."/>
          <TimelineBox  year="2023" title="Nissan" desc="I worked on the Backend of the website."/>
        </div>

        <img class="experience-timeline__image" src="../assets/images/diploma3d.png" alt="man with diploma">
      </div>

    </div>
  </section>
</template>

<script>
import TimelineBox from "@/components/TimelineBox";
import HeadingIcon from "@/components/HeadingIcon";

export default {
  name: "ExperienceSection",
  components:{
    TimelineBox,
    HeadingIcon
  }
}
</script>

<style lang="scss" scoped>
  .experience{

    .experience-wrapper{
      background: url("../assets/images/backgrounds/work4.png");
      background-size: cover;
      max-width: var(--container-width);
      margin: 50px auto 0;

      .experience-timeline {
        margin-top: 20px;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-column-gap: 30px;
        position: relative;

        .experience-timeline__image{
          position: absolute;
          bottom: 0;
          height: 440px;
          right: 0;
          transform: translate(50%, 17%);
        }

        .experience-timeline-card-1{
        background: rgba(255, 255, 255, 0.06);
        border-radius: 16px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        backdrop-filter: blur(2.5px);
        -webkit-backdrop-filter: blur(2.5px);
        border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .experience-timeline-card-2{
          /* From https://css.glass */
          background: rgba(255, 255, 255, 0.2);
          border-radius: 16px;
          box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
          backdrop-filter: blur(5px);
          -webkit-backdrop-filter: blur(5px);
          border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .timeline {
          width: 400px;
          height: 136px;
          //background: gray;
          margin-bottom: 30px;



          &:before {
            position: absolute;
            content: '';
            width: 1px;
            height: 84%;
            bottom: 0;
            background: var(--color-main);
            transform: translateX(-50%);
            border-radius: 20px;
          }

        }
      }
    }



  }
</style>