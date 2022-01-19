<template>
  <div class="main">
    <div class="navigation">
      <input
        type="text"
        class="search"
        placeholder="City Name..."
        v-model="city"
        autofocus
      />
    </div>
    <div class="content">
      <h1 class="city">{{ city }}</h1>
      <h6 class="date">{{ day }} , {{ month }} {{ date }}, {{ year }}</h6>
      <h1 class="temperature">{{ temp }}°C</h1>
    </div>
    <div class="footer">
      <h1 class="weather">{{ weather }}</h1>
      <h2 class="temperatures">{{ minTemp }}°c/{{ maxTemp }}°c</h2>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const city = ref("Panagudi");
    const day = ref("Sunday");
    const month = ref("January");
    const date = ref(22);
    const year = ref(2022);
    const temp = ref(22);
    const minTemp = ref(18);
    const maxTemp = ref(25);
    const weather = ref("Cloudy");

    return {
      city,
      day,
      month,
      date,
      year,
      temp,
      minTemp,
      maxTemp,
      weather,
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=PT+Sans&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");
.main {
  height: 100vh;
  width: 100vw;
  background-image: url("../assets/cool.jpg");
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  /* justify-content: center; */
  padding: 5% 10%;
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
.content {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.city {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  font-size: 75px;
  color: #fff;
  height: 120px;
}
.date {
  font-family: "PT Sans", sans-serif;
  font-size: 20px;
  color: rgba(0, 0, 0, 0.5);
  height: 25px;
}
.temperature {
  font-family: sans-serif;
  text-transform: uppercase;
  font-size: 125px;
  color: #fff;
  padding: 10px;
  box-shadow: 1px 2px 25px rgba(0, 0, 0, 0.5);
  border-radius: 100% 0% 100% 0% / 100% 100% 100% 100% ;
  background-color: rgba(0, 0, 0, 0.048);
  margin-top: 20px;
  height: 170px;
}
.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 30px;
  height: 170px;
}
.footer .weather {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  font-size: 20px;
  color: #fff;
  margin-top: 20px;
}
.temperatures {
  font-family: sans-serif;
  font-size: 30px;
  color: #fff;
  margin-top: 20px;
}
</style>
