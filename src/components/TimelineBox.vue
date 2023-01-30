<template>
  <div class="timeline">
    <div class="timeline-icon">
      <img src="../assets/images/graduate.png" alt="graduation cap">
    </div>
    <div class="timeline-text">
      <div class="timeline-text__year">2019-present</div>
      <div class="timeline-text__title">Bachlor's Degree</div>
      <div class="timeline-text__desc">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem.</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TimelineBox",
  props:{
    year: String,
    title:String,
    desc: String,
  }
}
</script>

<style lang="scss" scoped>
    .timeline{
      position: relative;

      .timeline-icon {
        width: 35px;
        position: absolute;
        top: 0;
        transform: translate(-50%, -26%);
        img{
          width: inherit;
        }
      }

      .timeline-text{
        padding-left: 40px;

        .timeline-text__year{
          font-weight: 300;
        }

        .timeline-text__title{
          font-weight: 600;
          margin: 8px 0;
        }

        .timeline-text__desc{
          font-weight: 300;
        }
      }
    }
</style>