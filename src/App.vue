<template>
    <NavigationBar @hamburgerClick-event="hamburger_click"/>
    <MobileNavbarMenu v-bind:is_active="is_active"/>
    <SocialBar />
    <SecondCoverSection/>
    <ExpertiseSection/>
    <XperienceSection />
    <FooterBar/>
<!--    <ContactSection/>-->

</template>

<script>
import MobileNavbarMenu from "@/components/MobileNavbarMenu";
import SecondCoverSection from "@/components/SecondCoverSection";
import NavigationBar from "@/components/NavigationBar";
import ExpertiseSection from "@/components/ExpertiseSection";
// import ExperienceSection from "@/components/ExperienceSection";
import XperienceSection from "@/components/XperienceSection";
import SocialBar from "@/components/SocialBar";
import FooterBar from "@/components/FooterBar";


// import ContactSection from "@/components/ContactSection";

export default {
  name: 'App',
  components: {
    MobileNavbarMenu,
    NavigationBar,
    SecondCoverSection,
    ExpertiseSection,
    XperienceSection,
    SocialBar,
    FooterBar,
    // ContactSection: ContactSection
  },
  data(){
    return {
      is_active: '',
    }
  },
  methods:{
    hamburger_click(isHamburgerMenuOpen){
      console.log('event received: ' + isHamburgerMenuOpen);
      if(isHamburgerMenuOpen){
        this.is_active = 'active'
      }else{
        this.is_active = ''
      }
    }
  },
  mounted() {
    // document.title = "Nikhil Aukhaj";
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

  html{
    scroll-behavior: smooth;
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
