<template>
  <h1 >{{heading}}</h1>
</template>

<script>
export default {
  name: "HeadingBullet",
  props: {
    heading: String
  }
}
</script>

<style lang="scss" scoped>
h1{
  position: relative;
  z-index: 2;

  &:before{
      content: "";
      background-image: url('../assets/images/icons/abstract_icon_bulletpoint_2.svg');
      background-size: var(--heading-icon-size)  var(--heading-icon-size);
      width:  var(--heading-icon-size);
      height:  var(--heading-icon-size);
      position: absolute;
      top: 0;
      z-index: -1;
    transform: translateX(-130%);
  }
}
</style>