<template>
  <section class="xperience">
    <div class="xperience-wrapper">
      <div></div>
       <div class="xperience-content">
          <div class="xperience-content-box">
            <h1>Education</h1>
            <div class="xperience-content-box__details">
              <h3>2012</h3>
              <h5>Sir Leckraz Teelock SSS</h5>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem, reprehenderit?</p>
            </div>
            <div class="xperience-content-box__details">
              <h3>2019</h3>
              <h5>University Of Technology, Mauritius</h5>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem, reprehenderit?</p>
            </div>
          </div>
         <div class="xperience-content-box">
           <h1>Professional</h1>
             <div class="xperience-content-box__details">
               <h3>2022</h3>
               <h5>Publicis Groupe</h5>
               <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem, reprehenderit?</p>
             </div>
         </div>
       </div>
      <div></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "XperienceSection"
}
</script>

<style lang="scss" scoped>
  .xperience{
    height: auto;
    min-height:100vh;
    background-image: linear-gradient(to right, gold, orange);

    .xperience-wrapper{
      height: 100%;
      display: grid;
      padding: 30px 0;
      grid-template-columns: 1fr 5fr 1fr;

      .xperience-content{
        /* From https://css.glass */
        background: rgba(255, 255, 255, 0.2);
        border-radius: 16px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        backdrop-filter: blur(5px);
        -webkit-backdrop-filter: blur(5px);
        border: 1px solid rgba(255, 255, 255, 0.3);
        height: 100%;
        padding: 10px 40px;


        .xperience-content-box{
            h1{
              font-size: 4.1rem;
              font-weight: bold;
              opacity: 0.4;
              color: white;
              text-transform: uppercase;
            }

            .xperience-content-box__details{
              margin-bottom: 35px;
              padding-left: 20px;
              border-left: 4px solid black;

                h3{
                  font-size:3.1rem;
                }

                h5{
                  font-size: 2.1rem;
                  text-transform: uppercase;
                }

              p{
                color: #ffffffb0;
              }


            }
        }

      }
    }
  }

  //h3
  //font-size: 4.1rem;
  //font-weight: bold;
  //opacity: 0.4;
  //color: white;
  //text-transform: uppercase;
</style>