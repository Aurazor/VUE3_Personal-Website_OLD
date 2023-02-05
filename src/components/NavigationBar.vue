<template>
  <nav>
    <div class="nav-logo">
      NIKHIL AUKHAJ
    </div>
    <div class="nav-items">
      <div class="nav-items-link text-animate">Intro</div>
      <div class="nav-items-link text-animate">Skills</div>
      <div class="nav-items-link text-animate">Experience</div>
      <div class="nav-items-link rounded-link">Contact Me</div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavigationBar"
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

   .nav-logo{
     font-weight: bold;
     font-size: 1.3rem;
   }

   .nav-items{
     text-transform: uppercase;
     display: flex;
     align-items: center;

     .nav-items-link{
       display:inline-block;
       margin: 0 10px;
       cursor: pointer;
       transition: 0.4s ease;
       color: #3e3e3e;

       &:hover.text-animate{
         color: var(--color-primary);
       }
     }

     .rounded-link{
       background-color: var(--color-primary);
       color: white;
       padding: 5px 10px;
       border-radius: 20px;
     }
   }

 }
</style>