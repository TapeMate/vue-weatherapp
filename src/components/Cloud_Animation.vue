<template>
  <div class="animation-body">
    <div id="background-wrap">
      <div class="x1">
        <div class="cloud"></div>
      </div>

      <div class="x2">
        <div class="cloud2"></div>
      </div>

      <div class="x3">
        <div class="cloud2"></div>
      </div>

      <div class="x4">
        <div class="cloud3"></div>
      </div>

      <div class="x5">
        <div class="cloud3"></div>
      </div>

      <div class="x6">
        <div class="cloud3"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Cloud_Animation",
};
</script>

<style scoped>
.animation-body {
  position: absolute;
  z-index: 1;
  background: #00b4ff;
  color: #333;
  font: 100% Arial, Sans Serif;
  height: 50vh;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

#background-wrap {
  bottom: 0;
  left: 0;
  /* padding-top: 50px; */
  position: fixed;
  right: 0;
  top: 45%;
  z-index: -1;
}

/* KEYFRAMES */

@-webkit-keyframes animateCloud {
  0% {
    margin-left: -500px;
  }
  100% {
    margin-left: 100%;
  }
}

@-moz-keyframes animateCloud {
  0% {
    margin-left: -500px;
  }
  100% {
    margin-left: 100%;
  }
}

@keyframes animateCloud {
  0% {
    margin-left: -500px;
  }
  100% {
    margin-left: 100%;
  }
}

/* ANIMATIONS */

.x1 {
  animation: animateCloud 25s linear infinite;
  transform: scale(0.55);
}

.x2 {
  animation: animateCloud 14s linear infinite;
  transform: scale(0.3);
}

.x3 {
  animation: animateCloud 18s linear infinite;
  transform: scale(0.5);
}

.x4 {
  animation: animateCloud 11s linear infinite;
  transform: scale(0.4);
}

.x5 {
  animation: animateCloud 8s linear infinite;
  transform: scale(0.55);
}

.x6 {
  animation: animateCloud 6s linear infinite;
  transform: scale(0.25);
}

/* OBJECTS */

.cloud {
  background: grey;
  background: linear-gradient(top, #fff 5%, #f1f1f1 100%);
  border-radius: 100px;
  box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);

  height: 120px;
  position: relative;
  width: 350px;
}

.cloud2 {
  background: rgb(231, 231, 231);
  background: linear-gradient(top, #fff 5%, #f1f1f1 100%);
  border-radius: 100px;
  box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);

  height: 120px;
  position: relative;
  width: 350px;
}

.cloud3 {
  background: rgb(194, 194, 194);
  background: linear-gradient(top, #fff 5%, #f1f1f1 100%);
  border-radius: 100px;
  box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);

  height: 120px;
  position: relative;
  width: 350px;
}
.cloud:after,
.cloud:before {
  background: grey;
  content: "";
  position: absolute;
  z-index: -1;
}

.cloud:after {
  border-radius: 100px;
  height: 100px;
  left: 50px;
  top: -50px;
  width: 100px;
}

.cloud:before {
  border-radius: 200px;
  width: 180px;
  height: 180px;
  right: 50px;
  top: -90px;
}

.cloud2:after,
.cloud2:before {
  background: rgb(231, 231, 231);
  content: "";
  position: absolute;
  z-index: -1;
}

.cloud2:after {
  border-radius: 100px;
  height: 100px;
  left: 50px;
  top: -50px;
  width: 100px;
}

.cloud2:before {
  border-radius: 200px;
  width: 180px;
  height: 180px;
  right: 50px;
  top: -90px;
}

.cloud3:after,
.cloud3:before {
  background: rgb(194, 194, 194);
  content: "";
  position: absolute;
  z-index: -1;
}

.cloud3:after {
  border-radius: 100px;
  height: 100px;
  left: 50px;
  top: -50px;
  width: 100px;
}

.cloud3:before {
  border-radius: 200px;
  width: 180px;
  height: 180px;
  right: 50px;
  top: -90px;
}
</style>
