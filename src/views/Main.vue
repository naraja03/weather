<template>
  <div class="main">
    <div class="navigation">
      <input type="text" class="search" placeholder="City Name..." />
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

.navigation input {
  padding: 15px 50px;
  border-radius: 20px 20px 20px 40px;
  outline: none;
  border: none;
  background: #fff;
  color: #525865;
  /* border-radius: 4px;
  border: 1px solid #d1d1d1; */
  box-shadow: inset 1px 2px 8px rgba(0, 0, 0, 0.07);
}

input:hover {
  box-shadow: inset 1px 2px 8px rgba(0, 0, 0, 0.02);
}
input:focus {
  color: #4b515d;
  border: 1px solid #b8b6b6;
  box-shadow: inset 1px 2px 4px rgba(0, 0, 0, 0.01),
    0px 0px 8px rgba(0, 0, 0, 0.2);
}
</style>
