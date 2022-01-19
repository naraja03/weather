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
@import url("https://fonts.googleapis.com/css2?family=PT+Sans&display=swap");
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
  box-shadow: 1px 2px 12px rgba(0, 0, 0, 0.2);
  font-family: "PT Sans", sans-serif;
  font-size: 20px;
  text-transform: capitalize;
}

.navigation input:hover {
  color: #525865;
  box-shadow: 1px 2px 25px rgba(0, 0, 0, 0.3);
}
.navigation input:active {
  color: #525865;
  box-shadow: 1px 2px 25px rgba(0, 0, 0, 0.2);
}
</style>
