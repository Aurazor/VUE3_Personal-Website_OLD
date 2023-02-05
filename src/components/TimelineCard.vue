<template>
  <div class="timeline-card">
    <div class="timeline-card-year">
      <HeadingBullet v-bind:heading="year"/>
    </div>
    <div class="timeline-card-box" :class="icon">
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
    subtitle: String,
    icon: String
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
      box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
      position: relative;
      transition: 0.6s ease;
      border: 1px solid transparent;

      .timeline-card__header{
        margin-bottom: 15px;
        font-size: 1.2rem;
      }

      .timeline-card__subtitle{
        font-weight: 300;
      }

      &:hover{
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
      }

    }

    .timeline-card-icon{
      &:after{
        content:url('../assets/images/icons/timeline_card_icon.svg');
        width:  var(--timeline-card-icon-size);
        height:  var(--timeline-card-icon-size);
        position: absolute;
        top: 0;
        right: 0;
        transform: translate(0,-50%);
      }
    }
  }
</style>