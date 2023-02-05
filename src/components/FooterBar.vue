<template>
  <footer>
    &copy;2023 | Nikhil Aukhaj All Rights Reserved.
  </footer>
</template>

<script>
export default {
  name: "FooterBar"
}
</script>

<style lang="scss" scoped>
  footer{
    background: hsl(180deg, 5%, 95%);
    height: var(--footer-height);
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>