<template>
  <div class="container">
    <div class="location-and-toggle">
      <div class="location">
        <h1 class="name">Binh Phuoc - Viet Nam</h1>
        <h5 class="zone">2021/10/05-21:30:06|GMT-07</h5>
      </div>
      <div class="toggle">
        <h3>°C | °F</h3>
      </div>
    </div>
    <div class="detail-and-slider">
      <div class="detail">
        <h1 class="temp">23°C</h1>
        <h4 class="icon">🚀</h4>
        <h2 class="desc">light rainny</h2>
      </div>
      <span></span>
      <div class="slider"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  background: rgba(255, 255, 255, 0.315);
  width: 550px;
  height: 300px;
  border-radius: 15px;
  border: 3px solid white;
}
.location-and-toggle {
  display: flex;
  width: 550px;
  height: 90px;
  padding: 0;
}
.location {
  display: grid;
  width: 80%;
  height: 100%;
  word-wrap: normal;
}
.name,
.zone {
  width: 100%;
  text-align: start;
  padding: 0 20px;
}
.toggle {
  width: 20%;
  height: 100%;
  display: flex;
}
.detail-and-slider {
  width: 550px;
  height: 200px;
  display: flex;
  /* background: yellow; */
}
.detail {
  width: 60%;
  height: 100%;
  display: grid;
  justify-content: center;
  align-items: center;
}

.temp {
  font-size: 3rem;
  font-weight: bolder;
  margin-top: -15px;
}
span {
  width: 1px;
  border-left: 1px solid rgb(82, 82, 82);
  height: 60%;
}
.slider {
  width: 40%;
  height: 100%;
}
</style>
