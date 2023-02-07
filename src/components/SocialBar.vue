<template>
  <div class="social-bar">
    <div class="social-bar-img">
      <a href="https://www.facebook.com/nikhil.aukhaj/"> <img src="../assets/images/icons/facebook.png" alt="Facebook logo"></a>
    </div>
    <div class="social-bar-img">
      <a href="https://twitter.com/Aurazor_8"><img src="../assets/images/icons/twitter.png" alt="Twitter logo"></a>
    </div>
    <div class="social-bar-img">
      <a href="https://github.com/Aurazor"><img src="../assets/images/icons/github.png" alt="Github logo"></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "SocialBar"
}
</script>

<style lang="scss" scoped>
  .social-bar{
    z-index: 5;
    position: fixed;
    right: 0;
    top: 40%;
    padding: 10px 10px;
    /* From https://css.glass */
    background: rgba(255, 255, 255, 0.2);
    border-radius: 5px;
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(5px);
    -webkit-backdrop-filter: blur(5px);
    border: 1px solid rgba(255, 255, 255, 0.15);

    .social-bar-img{
      width: 40px;
      margin: 5px 0;
      cursor: pointer;

      img{
        width: 100%;
        transition: 0.4s ease;

        &:hover{
          transform: scale(1.5);
        }
      }
    }
  }

  @media only screen and (max-width:769px) {
    .social-bar{
      top: auto;
      bottom: 0;
      display: flex;
      padding: 6px 7px;
      border-radius: 3px;

      .social-bar-img{
        margin: 0 7px;
      }
    }
  }
</style>