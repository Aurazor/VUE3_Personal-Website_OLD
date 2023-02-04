<template>
  <div class="timeline-card">
    <div class="timeline-card-year">
      <HeadingBullet v-bind:heading="year"/>
    </div>
    <div class="timeline-card-box">
      <div class="timeline-card__header">
        {{ header }}
      </div>
      <div class="timeline-card__subtitle">
        {{ subtitle }}
      </div>
    </div>
  </div>
</template>

<script>
import HeadingBullet from "@/components/HeadingBullet";

export default {
  name: "TimelineCard",
  props:{
    year:String,
    header:String,
    subtitle: String
  },
  components:{
    HeadingBullet
  }
}
</script>

<style lang="scss" scoped>
  .timeline-card{
    padding-left: 40px;
    padding-bottom: 30px;

    .timeline-card-year{
      margin-bottom: 10px;
      font-weight: bold;
      font-size: 1.2rem;
    }

    .timeline-card-box{
      padding: 20px 30px;
      border-radius: 11px;
      background-color: white;
      box-shadow: rgb(0 0 0 / 15%) 1.95px 1.95px 2.6px;

      .timeline-card__header{
        margin-bottom: 15px;
        font-size: 1.2rem;
      }

      .timeline-card__subtitle{
        font-weight: 300;
      }
    }
  }
</style>