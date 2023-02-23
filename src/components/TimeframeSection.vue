<template>
 <div class="timeframe">
   <div class="timeframe-wrapper">
     <div class="timeframe-img">
        <div class="timeframe-img__box">
          <img src="../assets/images/diploma3d.png" alt="Diploma image">
        </div>
     </div>
     <div class="timeframe-area">

     </div>
   </div>
 </div>
</template>

<script>
export default {
  name: "TimeframeSection",
  data() {
    return {
      "timeline": [
        {
          "name": "Education",
          "experience": [
            {
              "year": "2012",
              "place": "Sir Leckraz Teelock SSS",
              "details": "Lorem ipsum 1234"
            },
            {
              "year": "2019",
              "place": "University Of Technology, Mauritius",
              "details": "Lorem ipsum 1234"
            }
          ]
        },
        {
          "name": "Professional",
          "experience": [
            {
              "year": "2022",
              "place": "Publicis Groupe",
              "details": "Lorem ipsum 1234"
            }
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  .timeframe{
    .timeframe-wrapper{
      .timeframe-img{

      }

      .timeframe-area{

      }
    }
  }
</style>