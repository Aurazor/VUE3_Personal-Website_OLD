<template>
  <div class="timeline">
    <div class="timeline-icon">
      <img src="../assets/images/cap.png" alt="graduation cap">
    </div>
    <div class="timeline-text">
      <div class="timeline-text__year">{{year}}</div>
      <div class="timeline-text__title">{{title}}</div>
      <div class="timeline-text__desc">{{desc}}</div>
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
        padding-left: 30px;

        .timeline-text__year{
          font-weight: 300;
          color: var(--color-primary);
        }

        .timeline-text__title{
          margin: 8px 0;
          font-size: 1.2rem;
          text-transform: uppercase;
        }

        .timeline-text__desc{
          font-weight: 300;
        }
      }
    }
</style>