<template>
  <div class="mobile-nav-menu">
    <div class="nav-items">
      <div class="nav-items-link"><a class="text-animate" href="#second-intro">Intro</a> </div>
      <div class="nav-items-link"><a class="text-animate" href="#expertise">Skills</a></div>
      <div class="nav-items-link"><a class="text-animate" href="#experience">Experience</a></div>
      <div class="nav-items-link rounded-link rounded-link-1"><a href="#">Contact</a></div>
      <div class="nav-items-link rounded-link rounded-link-2"><a href="@/assets/documents/CV_Nikhil_Aukhaj.pdf">Download CV</a></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MobileNavbarMenu"
}
</script>

<style lang="scss" scoped>
 .mobile-nav-menu{
   display: none;
   &.active{
     display: block;
     height: 100%;
     position: fixed;
     right: 0;
     width: 50%;
     background: white;
     z-index: 5;
     padding: 0 30px;
   }

   .nav-items{
     .nav-items-link{
       cursor: pointer;
       width: 100%;
       padding: 10px 10px ;
       //transition: 0.9s ease;
       border-radius: 10px;

       &:hover{
         background: var(--color-primary);
         color: white;
       }
     }
   }
 }
</style>