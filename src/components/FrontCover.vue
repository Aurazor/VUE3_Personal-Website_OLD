<template>
<section class="front-cover">
  <div class="front-cover-wrapper">

  <div class="front-cover-text">
    <h4>Hello,</h4>
    <h3>This is Nikhil Aukhaj</h3>
    <p>An ambitious software engineer in Mauritius.</p>
  </div>

  <div class="front-cover-img">
      <div class="img-box">
        <img src="../assets/images/icons/profile-avatar2.png" alt="Profile Avatar">
      </div>
  </div>
  </div>

</section>
</template>

<script>
export default {
  name: "FrontCover"
}
</script>

<style lang="scss" scoped>

.front-cover{
  //margin-top:var(--nav-height);
  //height: calc(100vh - var(--nav-height));
  height: 100vh;
  background: url("../assets/images/backgrounds/wall1.jpg");
  background-size: cover;
  display: grid;
  align-items: center;
  padding: 0 30px;


  .front-cover-wrapper {
    display: grid;
    grid-template-columns: 1.5fr 1fr;
    height: 82%;
    align-items: center;
    justify-items: center;
    padding: 0 40px;

    .front-cover-text {

    }

    .front-cover-img {

        .img-box{
          border: 1px solid black;
          border-radius: 50%;
          overflow: hidden;
          img{
            width: 100%;
            transform: translateY(8px);
          }
        }
    }
  }
}
</style>