<template>
  <section id="home" class="hero is-fullheight columns">
    <div class="home-bg">
      <div class="skew"></div>
      <div class="overlay"></div>
      <div class="bg-images"></div>
    </div>
    <div class="profile-images column"></div>
    <div class="title column">
      <h1 class="text-upper-case">
        amimul Ihsan
        <strong>Mahdi</strong>
      </h1>
      <vue-typed-js
        :strings="animText"
        :typeSpeed="100"
        :loop="true"
        :smartBackspace="true"
        :backDelay="1200"
        :backSpeed="20"
      >
        <p class="typing"></p>
      </vue-typed-js>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      animText: [
        "Programmer",
        "Software Engineer",
        "Android App Developer",
        "Native Android and Flutter Developer"
      ]
    };
  }
};
</script>

<style lang="scss">
#home {
  overflow: hidden;
  transition: all 340ms ease-in-out;
  display: flex;
  align-items: center;

  .home-bg {
    position: absolute;
    height: 100vh;
    height: 100%;
    right: -35px;
    top: 0;
    width: 50%;
    .skew {
      transform: skew(-15deg);
      height: 100vh;
      width: 55%;
      position: absolute;
      left: -230px;
      background-color: #fff;
      z-index: 1;
    }
    .overlay {
      background-color: rgba(85, 174, 161, 0.9);
      position: absolute;
      width: 100%;
      height: 100%;
    }
    .bg-images {
      background-image: url("../assets/images/programmer-coding.jpg");
      width: 100%;
      height: 100vh;
      background-size: 160%;
      background-size: cover;
      background-repeat: no-repeat;
    }
  }
  .profile-images {
    background-image: url("../assets/images/amimulislammahdi.jpg");
    width: 460px;
    height: 310px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(0%, -50%);
    border-radius: 5px;
    box-shadow: -7px -1px 18px rgba(193, 193, 193, 0.43);
    z-index: 2;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    transition: all 0.3s ease;
  }
  .title {
    position: absolute;
    top: 50%;
    margin-left: 4%;
    left: 200px;
    padding: 0;
    z-index: 3;
    font-weight: 500;
    h1 {
      font-size: 55px;
      color: #1e1e1e;
      position: relative;
      strong {
        font-weight: 700;
        color: rgba(85, 174, 161, 0.9);
      }
    }
    .text-upper-case {
      text-transform: uppercase;
    }
  }
}
</style>