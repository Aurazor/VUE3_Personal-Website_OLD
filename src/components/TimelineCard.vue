<template>
  <div class="timeline-card">
    <div class="timeline-card-year">
      <HeadingBullet v-bind:heading="year"/>
    </div>
    <div class="timeline-card-box" :class="icon">
      <div class="timeline-card__header highlight-text-timeline-header">
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
      position: relative;
      transition: 0.4s ease;
      border: 1px solid transparent;
      box-shadow: rgb(99 99 99 / 20%) 0px 2px 8px 0px;

      .timeline-card__header{
        margin-bottom: 15px;
        font-size: 1.2rem;
        font-weight: bold;
        display: inline-block;
        //font-size: 1.2rem;
        //display: inline-block;
        //padding: 4px 10px;
        //border-radius: 10px;
        //border: 1px solid gold;
        //font-weight: 600;
      }

      .timeline-card__subtitle{
        font-weight: 300;
      }

      &:hover{
        box-shadow: rgba(136, 165, 191, 0.48) 6px 2px 16px 0px, rgba(255, 255, 255, 0.8) -6px -2px 16px 0px;
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