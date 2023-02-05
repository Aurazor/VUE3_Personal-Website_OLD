<template>
    <NavigationBar/>
    <MobileNavbarMenu/>
    <SecondCoverSection/>
    <ExpertiseSection/>
    <ExperienceSection />
    <FooterBar/>
<!--    <ContactSection/>-->

</template>

<script>
import MobileNavbarMenu from "@/components/MobileNavbarMenu";
import SecondCoverSection from "@/components/SecondCoverSection";
import NavigationBar from "@/components/NavigationBar";
import ExpertiseSection from "@/components/ExpertiseSection";
import ExperienceSection from "@/components/ExperienceSection";
import FooterBar from "@/components/FooterBar";
// import ContactSection from "@/components/ContactSection";

export default {
  name: 'App',
  components: {
    MobileNavbarMenu,
    NavigationBar,
    SecondCoverSection,
    ExpertiseSection,
    ExperienceSection,
    FooterBar
    // ContactSection: ContactSection
  },
  mounted() {
    document.title = "Nikhil Aukhaj";
  },
}
</script>

<style lang="scss">
  @import './assets/_helpers/scss/_variables.scss';
  @import './assets/_helpers/scss/custom_styles.scss';

  @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,300;0,400;0,600;0,700;1,400&display=swap');

  *{
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }

  body{
    font-family: 'Poppins', sans-serif;
    position: relative;
    overflow-x:hidden;

  }

  section{
    min-height: 100vh;
  }

  a{
    text-decoration: none;
    color: black;
  }

  ul{
    list-style: none;
  }

  .app-container{
    max-width: var(--container-width) ;
    margin: 0 auto;
  }


</style>
