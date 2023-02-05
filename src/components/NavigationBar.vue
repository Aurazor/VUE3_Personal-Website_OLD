<template>
  <nav>
    <div class="nav-brand">
      <div class="nav-brand-logo">
        <img src="../assets/images/icons/lion_logo_1.png" alt="Lion Logo">
      </div>
      <div class="nav-brand-text">
        NIKHIL AUKHAJ
      </div>
    </div>
    <div class="nav-items">
      <div class="nav-items-link"><a class="text-animate" href="#second-intro">Intro</a> </div>
      <div class="nav-items-link"><a class="text-animate" href="#expertise">Skills</a></div>
      <div class="nav-items-link"><a class="text-animate" href="#experience">Experience</a></div>
      <div class="nav-items-link rounded-link"><a href="">Contact</a></div>
    </div>
    <div class="nav-hamburger-menu"  v-on:click="handleClick">
      <img class="nav-hamburger-menu__img" src="../assets/images/icons/hamburger.png" alt="mobile menu icon">
    </div>
  </nav>
</template>

<script>
import {mobileNavbarHamburgerClick} from '../assets/custom_scripts/mobile_nav';

export default {
  name: "NavigationBar",
  methods:{
    handleClick(){
      mobileNavbarHamburgerClick()
    }
  }

}
</script>

<style lang="scss" scoped>
 nav{
   background: white;
   position: fixed;
   top: 0;
   width: 100%;
   display: flex;
   justify-content: space-between;
   align-items: center;
   height: var(--nav-height);
   padding: 0 30px;
   z-index: 3;
   box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;

   .nav-brand{
     font-weight: bold;
     font-size: 1.3rem;
     display: flex;
     justify-content: center;
     align-items: center;

     .nav-brand-logo{
       display: flex;
       justify-content: center;
       align-items: center;
       width: 30px;
       margin-right: 10px;

       img{
         width: 100%;
       }
     }

   }

   .nav-items{
     text-transform: uppercase;
     display: flex;
     align-items: center;

     .nav-items-link{
       display:inline-block;
       margin: 0 10px;
       cursor: pointer;
       color: #3e3e3e;

        a{
          transition: 0.4s ease;

          &:hover.text-animate{
            color: var(--color-primary);
          }
        }

     }

     .rounded-link{
       background-color: var(--color-primary);
       padding: 5px 20px;
       border-radius: 20px;

       a{
         color: white;
       }
     }
   }

   .nav-hamburger-menu{
     display: none;
   }
 }

 @media only screen and (max-width:769px) {
   nav {
     .nav-items {
       display: none;
     }

     .nav-hamburger-menu {
       width: 30px;
       display: flex;
       justify-content: center;
       align-items: center;
       cursor: pointer;

       .nav-hamburger-menu__img {
         width: 100%;
       }
     }
   }
 }
</style>