<template>
 <h1>{{heading}}</h1>
</template>

<script>
export default {
  name: "HeadingIcon",
  props:{
    heading:String,
  }
}
</script>

<style lang="scss" scoped>
  h1{
    position: relative;
    font-size: 2.8rem;
    z-index: 2;

    &:before{
      content: "";
      background-image: url('../assets/images/icons/abstract_icon_2.svg');
      background-size: var(--heading-icon-size)  var(--heading-icon-size);
      filter: hue-rotate(180deg);
      width:  var(--heading-icon-size);
      height:  var(--heading-icon-size);
      position: absolute;
      top: 0;
      z-index: -1;
      transform: translate(-50%, -70%);
    }
  }
</style>