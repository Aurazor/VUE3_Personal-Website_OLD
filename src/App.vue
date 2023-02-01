<template>

    <NavigationBar/>
    <div class="app-container">
      <SecondCoverSection/>
      <ExpertiseSection/>
      <ExperienceSection/>
      <ContactSection/>
    </div>

</template>

<script>
import SecondCoverSection from "@/components/SecondCoverSection";
import NavigationBar from "@/components/NavigationBar";
import ExpertiseSection from "@/components/ExpertiseSection";
import ExperienceSection from "@/components/ExperienceSection";
import ContactSection from "@/components/ContactSection";

export default {
  name: 'App',
  components: {
    NavigationBar,
    SecondCoverSection,
    ExpertiseSection,
    ExperienceSection,
    ContactSection: ContactSection
  }
}
</script>

<style lang="scss">
  @import './assets/_helpers/scss/_variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,300;0,400;0,600;0,700;1,400&display=swap');
  /*@import 'assets/_helpers/custom_fonts.css';*/
  *{
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }

  body{
    font-family: 'Poppins', sans-serif;
    position: relative;
  }

  section{
    height: calc(100vh - 40px);
  }

  ul{
    list-style: none;
  }

  .app-container{
    max-width: var(--max-width) ;
    margin:0 auto;
  }

  //@media (min-width: 1280px){
  //  $width : 1280px;
  //  :root {
  //    --max-width: 1280px;
  //  }
  //}
  //
  //@media (min-width: 1024px){
  //  $width : 1024px;
  //  :root {
  //    --max-width: 1024px;
  //  }
  //}
  //
  //@media (min-width: 769px){
  //  $width : 769px;
  //  :root {
  //    --max-width: 769px;
  //  }
  //}
  //
  //@media (min-width: 640px){
  //  $width : 640px;
  //  :root {
  //    --max-width: 640px;
  //  }
  //}


</style>
