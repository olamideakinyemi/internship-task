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
            <div class="shadow-container">
                <div class="shadow">
                    <img src="./assets/images/model.png" alt="/" />
                </div>
            </div>
            <div class="logo">
                <div>
                    <img class="social" src="./assets/svg/instagram.svg" alt="/" />
                </div>
                <div>
                    <img class="social" src="./assets/svg/twitter.svg" alt="/" />
                </div>
                <div>
                    <img class="social" src="./assets/svg/snapchat.svg" alt="/" />
                </div>
                <div>
                    <img class="social" src="./assets/svg/email.svg" alt="/" />
                </div>
            </div>

            <div class="routes">
                <div>
                    <p>HOME</p>
                </div>
                <div>
                    <p>ABOUT</p>
                </div>
                <div>
                    <img class="image" src="./assets/images/profile.jpg" alt="/" />
                </div>
                <div>
                    <p>GALLERY</p>
                </div>
                <div>
                    <p>CONTACT</p>
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
    color: white;
    width: 50%;
    margin: auto;
    margin-top: 15px;
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

@media screen and (max-width: 425px) {
  .routes{
    margin-left: 20px;
  }
}
</style>
