<template>
  <div class="main">
    <div class="navigation">
      <input type="text" class="search" placeholder="City Name...">
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main {
  height: 100vh;
  width: 100vw;
  background-image: url("../assets/common.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  /* justify-content: center; */
  padding: 10%;
  align-items: center;
}

input .search{
  padding: 10px;
}
</style>
