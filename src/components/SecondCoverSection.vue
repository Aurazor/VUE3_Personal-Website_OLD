<template>
  <section class="second-cover" id="second-intro">
     <div class="second-cover-wrapper app-container">
       <div class="second-cover-text flex-center-vertical">
         <div class="second-cover-text__subtitle">Hello</div>
         <div class="second-cover-text__title">This is <span class="highlight-text">Nikhil Aukhaj</span></div>
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
       <div class="second-cover-img flex-center-vertical">
         <img src="../assets/images/leo.png" alt="second profile cover image">
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
    margin-top:var(--nav-height);
    height: calc(100vh - var(--nav-height));
    .second-cover-wrapper{
      height: 100%;
      display:grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 40px;
      padding: 50px 0;

      .second-cover-text{
        font-weight: 300;

        .second-cover-text__subtitle{
          font-size: 2rem;
        }

        .second-cover-text__title{
          font-size: 2.9rem;
          font-weight: 700;
          line-height: 50px;
          margin-top: 18px;
          margin-bottom: 24px;
        }

        .second-cover-test__list{
          font-size: 1.2rem;
          ul{
            li{
              text-transform: uppercase;
              margin-bottom: 10px;
            }
          }
        }

      }

      .second-cover-img{
        img{
          width: 100%;
          border-radius: 20px;
        }
      }
    }
  }

  @media only screen and (max-width:769px) {
    .second-cover{
      height: auto;

      .second-cover-wrapper{
        grid-template-columns: 1fr;

        .second-cover-text{
          text-align: center;
          text-transform: uppercase;

          .second-cover-text__title{
            line-height: 40px;
            font-size: 2.6rem;
          }
          .second-cover-text__subtitle{
            font-size: 1.6rem;
          }
        }

        .second-cover-img{
          display: flex;
          justify-content: center;
          align-items: center;
          grid-row: 1;

          img{
            width: 75%;
          }
        }
      }
    }
  }
</style>