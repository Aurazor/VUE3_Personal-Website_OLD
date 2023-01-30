<template>
 <section class="expertise">
   <div class="expertise-wrapper">
     <div class="expertise-img-container">
       <img src="../assets/images/second_cover.jpg" alt="Expertise Images">
     </div>
     <div class="expertise-text">
       <div class="expertise-text__title">
         My mission is to develop best design.
       </div>
       <div class="expertise-text__subtitle">I will help you build and grow your business. I create clarifying strategy, websites and mobile apps.</div>
       <div class="expertise-text__details">
         <div class="expertise-text__details-skill">
            <div class="expertise-text__details-skill-header">
              <div class="expertise-header-description">Web Design</div>
              <div class="expertise-header-percentage">90%</div>
            </div>
           <div class="expertise-text__details-skill-progress">
             <div id="expertise-progress-1" class="expertise-progress"></div>
           </div>
         </div>
         <div class="expertise-text__details-skill">
           <div class="expertise-text__details-skill-header">
             <div class="expertise-header-description">Mobile App Design</div>
             <div class="expertise-header-percentage">80%</div>
           </div>
           <div class="expertise-text__details-skill-progress">
             <div id="expertise-progress-2" class="expertise-progress"></div>
           </div>
         </div>
         <div class="expertise-text__details-skill">
           <div class="expertise-text__details-skill-header">
             <div class="expertise-header-description">Desktop Apps</div>
             <div class="expertise-header-percentage">85%</div>
           </div>
           <div class="expertise-text__details-skill-progress">
             <div id="expertise-progress-3" class="expertise-progress"></div>
           </div>
         </div>
       </div>
     </div>
   </div>
 </section>
</template>

<script>
export default {
  name: "ExpertiseSection"
}
</script>

<style lang="scss" scoped>
  .expertise{
    .expertise-wrapper{
      padding: 0 5%;
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-column-gap: 50px;
      align-items: center;
      height: 100%;

      .expertise-img-container{
        justify-self: center;
      }

      .expertise-text{
        .expertise-text__title{
          font-weight: 600;
          font-size: 45px;
          line-height: 45.2px;
        }

        .expertise-text__subtitle{
          font-weight: 300;
          margin-top: 20px;
          margin-bottom: 25px;
        }

        .expertise-text__details{
          .expertise-text__details-skill{
            .expertise-text__details-skill-header {
              display: flex;
              justify-content: space-between;
              align-items: center;
              text-transform: uppercase;
              font-weight: 600;
            }
              .expertise-text__details-skill-progress{
                width: 100%;
                height: 10px;



                .expertise-progress{
                  width: inherit;
                  height: inherit;
                  background: #e9e9e9;
                  position: relative;
                  border-radius: 10px;

                  &:after{
                    content: '';
                    background: red;
                    height: inherit;
                    position: absolute;
                    top: 0;
                    border-radius: 10px;
                  }
                }

                #expertise-progress-1{
                  &:after{
                    width: 90%;
                  }
                }

                #expertise-progress-2{
                  &:after{
                    width: 80%;
                  }
                }

                #expertise-progress-3{
                  &:after{
                    width: 85%;
                  }
                }

              }

          }
        }
      }

    }
  }
</style>