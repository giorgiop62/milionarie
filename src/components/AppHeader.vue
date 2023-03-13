<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="logo">
      <img src="/logo.png" alt="logo" />
    </div>
  </header>
</template>

<style lang="scss" scoped>
header{
    height: 300px;
    width: 100%;
    background-color: rgb(22 25 139);
}
img {
  width: 250px;
}
.logo {
  line-height: 300px;
  text-align: center;
  padding-top: 30px;

}
</style>