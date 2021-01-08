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
      <div class="routes">
        <p>HOME</p>
        <p>ABOUT</p>
        <div>
          <img class="image" src="./assets/images/profile.jpg" alt="/" />
        </div>
        <p>GALLERY</p>
        <p>CONTACT</p>
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
  box-shadow: -7px 0 5px 5px #940c3c;
  background: #ae1a4e;
  margin-left: 400px;
  padding-top: 60px;
  padding-left: 50px;
  padding-right: 50px;
}
.routes {
  display: flex;
  justify-content: between;
  align-items: center;
    text-align: center;
  font-size: 20px;
  color: white;
  margin-left: 510px;
  margin-top: 30px;
}
.image {
width: 130px;
height: 120px;
border-radius: 50%;
}
</style>
