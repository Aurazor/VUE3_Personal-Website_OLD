<template>
  <section class="contact">
    <div class="contact-wrapper">
      <div class="contact-heading">
        <HeadingIcon heading="Contact Me"/>
        <img src="../assets/images/plane_paper.png" alt="plane paper">
      </div>

      <div class="contact-view">
        <div class="contact-desc">
          <h3>Let's Talk About Everything!</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
        <div class="contact-form">
          <form action="#">
            <div class="contact-form__personal-details">
              <input type="text" placeholder="Your name" class="form-input">
              <input type="email" placeholder="Email Address" class="form-input">
            </div>
            <div class="contact-form__subject">
              <input type="text" placeholder="Subject" class="form-input">
            </div>
            <div class="contact-form__message">
              <textarea rows="10" class="form-input" placeholder="Message"/>
            </div>
            <button class="contact-form__btn-submit form-input" type="submit">Send Message</button>
          </form>
        </div>
    </div>
    </div>
  </section>
</template>

<script>
import HeadingIcon from "@/components/HeadingIcon";
export default {
  name: "ContactSection",
  components:{
    HeadingIcon
  },
  mounted() {
    document.title = 'Nikhil Aukhaj'
  }

}
</script>

<style lang="scss" scoped>
  .contact{
    .contact-wrapper{
      max-width: var(--container-width);
      margin: 0 auto;
      padding: 60px 0;
      height: 100%;

      .contact-heading{
        position: relative;

        img{
          position: absolute;
          top: 0;
          left: 25%;
          width: 104px;
          z-index: -1;

        }
      }
      .contact-view{
        display:grid;
        grid-template-columns: 1fr 2fr;
        margin-top: 18px;
        .contact-desc{
          p{
            font-weight: 300;
          }
        }

        .contact-form{
          form{
            .form-input{
              padding: 13px;
              border-radius: 20px;
              outline: none;
              border: none;
              box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 1px 3px 1px;
              width: 100%;
              font-family: 'Poppins', sans-serif;

              &::placeholder{
                font-weight: 300;
              }
            }
            .contact-form__personal-details{
              display:grid;
              grid-template-columns: 1fr 1fr;
              grid-column-gap: 10px;

            }

            .contact-form__subject{
              margin: 20px 0;
            }

            .contact-form__message{
              textarea{
                resize: none;
              }
            }

            .contact-form__btn-submit{
              background: var(--color-primary);
              color: white;
              width: auto;
              font-weight: bold;
              border-radius: 25px;
              padding: 12px 32px;
              margin-top: 15px;
            }
          }
        }
      }

    }
  }
</style>