<template>
  <div>
    <div class="bg">
      <div class="background"></div>
      <div class="background2"></div>
    </div>
    <div class="container">
      <div class="text">
        <p>{{ name }}</p>
      </div>
      <div class="shadow-container">
        <div class="shadow">
          <img src="./assets/images/model.png" alt="/" />
        </div>
      </div>
      <div class="logo">
        <div>
          <a :href="`https://instagram.com/${instagram}`">
            <img class="social" src="./assets/svg/instagram.svg" alt="/" />
          </a>
        </div>
        <div>
          <a :href="`https://twitter.com/${twitter}`"
            ><img class="social" src="./assets/svg/twitter.svg" alt="/" />
          </a>
        </div>
        <div>
          <a :href="`https://snapchat.com/${snapchat}`"
            ><img class="social" src="./assets/svg/snapchat.svg" alt="/" />
          </a>
        </div>
        <div>
          <a :href="`mailto:${email}`">
            <img class="social" src="./assets/svg/email.svg" alt="/" />
          </a>
        </div>
      </div>

      <div class="routes">
        <div>
          <a href="/home"> <p>HOME</p> </a>
        </div>
        <div>
         <a href="/about"> <p>ABOUT</p> </a>
        </div>
        <div>
          <img class="image" src="./assets/images/profile.jpg" alt="/" />
        </div>
        <div>
         <a href="/gallery"> <p>GALLERY</p>  </a>
        </div>
        <div>
          <a href="/contact"> <p>CONTACT</p>  </a>
        </div>
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

.shadow-container {
  display: flex;
  justify-content: center;
}

.shadow {
  display: flex;
  justify-content: center;
  width: 500px;
  height: 600px;
  box-shadow: -7px 0 5px 5px #940c3c;
  background: #ae1a4e;
  padding-top: 60px;
  padding-left: 50px;
  padding-right: 50px;
}

.routes {
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-align: center;
  font-size: 20px;

  width: 50%;
  margin: auto;
  margin-top: 15px;
}
.routes a {
  text-decoration: none;
  color: white;
}
.image {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  margin-left: 30px;
}
.social {
  width: 35px;
  margin-top: 25px;
  margin-right: 8px;
}

.logo {
  position: absolute;
  top: 0;
  right: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100%;
}

@media screen and (max-width: 640px) {
  .shadow {
    width: 100%;
  }
  .shadow img {
    width: 100%;
  }
  .bg {
    height: 100%;
  }
  .background,
  .background2 {
    height: 100%;
  }
}

@media screen and (max-width: 768px) {
  .routes {
    width: 100%;
    flex-direction: column;
    justify-content: center;
  }
}
</style>

<script>
export default {
  data() {
    return {
      name: "",
      instagram: "",
      twitter: "",
      snapchat: "",
    };
  },

  mounted() {
    fetch("https://hirng-x2021.glitch.me/api")
      .then((response) => response.json())
      .then((data) => {
        console.log(data);
        this.name = data.name;
        this.instagram = data.social_media.instagram;
        this.twitter = data.social_media.twitter;
        this.snapchat = data.social_media.snapchat;
        this.email = data.social_media.email;
      });
  },
};
</script>
