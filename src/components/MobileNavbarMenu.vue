<template>
  <div class="mobile-nav-menu">
    <ul>
      <li>Home</li>
      <li>About</li>
    </ul>
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
   }
 }
</style>