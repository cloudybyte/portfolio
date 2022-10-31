<template>
  <div class="wrapper-container container">
    <div class="wrapper-item">
      <p>element one</p>
    </div>
    <div class="wrapper-item">
      <div class="card">
        <h1>Projects</h1>
      </div>
    </div>
  </div>
  <!--<div class="container">
  </div>-->
</template>

<script>
export default {
  head () {
    return {
      bodyAttrs: {
        class: 'reset-body'
      }
    }
  }
}
</script>

<style >
@font-face {
  font-family: "Inconsolata";
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: url("~/assets/fonts/inconsolata/Inconsolata-Black.ttf") format('truetype');
}
.reset-body {
  margin: 0 !important;
}

.wrapper-container {
  height: 100vh;

  background-image: url("~assets/topography.svg");
  background-position: center center;
  background-repeat:  no-repeat;
  background-size:  cover;
  
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}
.wrapper-item {
  display: inline-grid;
  /*border: 1px solid red;*/
  align-items: center;
  text-align: center;
  font-family: 'Inconsolata';
}
.card {
  margin-right: auto;
  margin-left: auto;
  width: 60%;
  box-shadow: 0 15px 25px rgba(129, 124, 124, 0.2);
  height: 85%;
  border-radius: 20px;
  backdrop-filter: blur(10px);
  background-color: rgba(255, 255, 255, 0.2);
  padding: 10px;
  text-align: center;
}
</style>