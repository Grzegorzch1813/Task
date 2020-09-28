<template>
  <div class="container">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
width:1280px;
max-width:100%;
margin:0 auto;
}

.journey-section {
margin-top:50px;
position:relative;
}
</style>
