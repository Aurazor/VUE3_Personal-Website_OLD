<template>
  <section class="second-cover">
     <div class="second-cover-wrapper">
       <div class="second-cover-text">
         <div class="second-cover-text__subtitle">My Specialization</div>
         <div class="second-cover-text__title">I am a trending<br> developer who cares <br>about the details</div>
         <div class="second-cover-test__list">
           <ul>
             <li>01. Web Design</li>
             <li>02. Mobile Design</li>
             <li>03. Product Design</li>
             <li>04. Commercial Design</li>
             <li>05. Landscape Design</li>
           </ul>
         </div>
       </div>
       <div class="second-cover-img">
         <img src="../assets/images/second_cover.jpg" alt="second profile cover image">
       </div>
     </div>
  </section>
</template>

<script>
export default {
  name: "SecondCoverSection"
}
</script>

<style lang="scss" scoped>
  .second-cover{
    .second-cover-wrapper{
      height: 100%;
      display:grid;
      grid-template-columns: 1fr 1fr;
      align-items: center;

      .second-cover-text{
        font-weight: 300;
        .second-cover-text__title{
          font-weight: 600;
          font-size: 40px;
          line-height: 43px;
          margin-top:30px;
          margin-bottom: 50px;
        }

        .second-cover-test__list{
          ul{
            li{
              text-transform: uppercase;
              margin-bottom: 10px;
            }
          }
        }

      }

      .second-cover-img{
        justify-self: center;
      }
    }
  }
</style>