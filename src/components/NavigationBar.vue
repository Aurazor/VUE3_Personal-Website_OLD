<template>
  <nav>
    <div class="nav-logo">
      NIKHIL.
    </div>
    <div class="nav-email">
      nikhilaukhaj590@gmail.com
    </div>
    <div class="nav-icon">
      <img src="../assets/images/hamburger.png" alt="navigation icon">
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
   -webkit-box-shadow:0px 1px 1px #101010;
   -moz-box-shadow:0px 1px 1px #101010;
   box-shadow:0px 1px 1px #101010;
   z-index: 2;

   .nav-logo{
     font-weight: 600;
   }
   .nav-email{
     font-weight: 300;
   }

   .nav-icon{
     width: 24px;

     img{
       width: 100%;
     }
   }
 }
</style>