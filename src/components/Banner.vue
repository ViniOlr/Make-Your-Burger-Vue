<template>
  <div class="banner">
    <h1>Make Your Burguer</h1>
  </div>
</template>

<script>
export default {
    name: "Banner"
}
</script>

<style>
.banner {
  background-image: url('../../public/img/burger-banner.jpg');
  background-position: 0 -275px;
  background-size: cover;
  background-repeat: no-repeat;

  width: 100%;
  height: 475px;
}
.banner h1 {
  font-size: 3.3em;
  color: #ccc;
  background-color: rgba(0, 0, 0, 0.7);
  padding: 15px;
  display: inline-block;
  position: relative;
  top: 50%;
  transform: translateY(-50%);
}
</style>