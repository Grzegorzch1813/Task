<template>
  <div id="navigation">
    <ul>
      <li>ZAPLANUJ WYCIECZKĘ</li>
      <li>ATRAKCJE REGIONU</li>
    </ul>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#navigation {
  display: flex;
  width: 100%;
  margin-bottom: 50px;
  justify-content:center;
  align-items:center;
  ul {
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0 20px 0 0;
    li {
      font-size: 15px;
      padding: 2px 10px;
      cursor: pointer;
      &:hover {
        color: #7ca971;
      }
    }
  }
}
</style>
