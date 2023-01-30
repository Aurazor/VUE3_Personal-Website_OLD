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
  margin:20px 0;
  position: relative;

  &:before{
    background-image: url("../assets/images/square_dots.png");
    background-size: 35px 35px;
    width: 35px;
    height: 35px;
    content: "";
    position: absolute;
    top: 0;
    transform: translate(-45%, -25%);
    z-index: -1;
    opacity: 0.05;
  }
}
</style>