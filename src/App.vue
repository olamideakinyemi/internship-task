<template>
  <div>
    <div class="bg">
      <div class="background"></div>
      <div class="background2"></div>
    </div>
    <div class="container">
      <div class="text">
        <p>AQUILA AVEION</p>
      </div>
      <div class="shadow">
        <img src="./assets/images/model.png" alt="/" />
      </div>
    </div>
  </div>
</template>

<style>
.bg {
  position: fixed;
  top: 0;
  display: flex;
}
.background {
  background-color: #bd0f4d;
  width: 50vw;
  height: 100vw;
}
.background2 {
  background-color: #cb2964;
  width: 50vw;
  height: 100vw;
}
.container {
  position: relative;
  z-index: 800;
}
.text {
  text-align: center;
  font-size: 50px;
  color: white;
  word-spacing: 25px;
}
img {
 width: 350px;
}
.shadow {
   display: flex;
   justify-content: center;
   width: 500px;
   box-shadow: -7px 0 5px 5px #940C3C;
   background: #AE1A4E;
   margin-left: 400px;
   padding-top: 60px;
   padding-left: 50px;
 padding-right: 50px;
}
</style>
box-shadow: 10px 10px 5px #940C3C;
 padding-top: 60px;
 padding-left: 100px;
 padding-right: 100px;