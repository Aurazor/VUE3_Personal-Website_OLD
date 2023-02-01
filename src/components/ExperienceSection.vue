<template>
  <section class="experience">
    <div class="experience-wrapper">
     <HeadingIcon heading="Experience"/>
      <div class="experience-timeline">
        <div class="experience-education experience-timeline-card">
          <TimelineBox/>
          <TimelineBox/>
          <TimelineBox/>
        </div>
        <div class="experience-professional experience-timeline-card">
          <TimelineBox/>
          <TimelineBox/>
        </div>
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

      h1{
        margin:20px 0;
        position: relative;

        &:before{
          background-image: url("../assets/images/square_dots.png");
          background-size: 35px 35px;
          width: 35px;
          height: 35px;
          content: "";
          position: absolute;
          top: 0;
          transform: translate(-45%, -25%);
          z-index: -1;
          opacity: 0.05;
        }
      }
      .experience-timeline {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-column-gap: 30px;
        justify-content: center;

        .experience-timeline-card{
          border-radius: 20px;
          padding: 31px 37px;
          box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
        }

        .timeline {
          width: 400px;
          height: 136px;
          //background: gray;
          margin-bottom: 30px;

          &:before {
            position: absolute;
            content: '';
            width: 2px;
            height: 95px;
            bottom: 0;
            background: red;
            transform: translateX(-50%);
          }

        }
      }
    }



  }
</style>