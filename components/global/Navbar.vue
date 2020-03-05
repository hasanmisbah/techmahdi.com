<template>
  <div>
    <nav class="main-nav fixed-top">
      <div class="logo">
        <a href="#">
          <span class="logo_bg"></span>
        </a>
      </div>
      <div class="container">
        <div class="nav-wrapper">
          <ul class="navigation">
            <li>
              <nuxt-link to="/">
                <i class="fas fa-home"></i>
                <span>Home</span>
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/about">
                <i class="fa fa-user"></i>
                <span>About</span>
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">
                <i class="fas fa-layer-group"></i>
                <span>Service</span>
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">
                <i class="far fa-image"></i>
                <span>Portfolio</span>
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">
                <i class="fa fa-comment-dots"></i>
                <span>Testimonials</span>
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="#">
                <i class="fa fa-envelope"></i>
                <span>Contact</span>
              </nuxt-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="social-media">
        <ul>
          <li>
            <a href="#">
              <i class="fab fa-facebook-f"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fab fa-twitter"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fab fa-linkedin"></i>
            </a>
          </li>
          <li>
            <a href="#">
              <i class="fab fa-instagram"></i>
            </a>
          </li>
        </ul>
        <div class="container">
          <p class="thin">Amimul Ihsan Mahdi &copy; 2020</p>
          <p class="thin">
            Developed By :
            <a href="https://github.com/hasanmisbah">Hasan Misbah</a>
          </p>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: true
    };
  }
};
</script>

<style lang="scss">
.nav-toggle {
  width: 27px;
  height: 21px;
  position: absolute;
  top: 0;
  left: 2px;
  bottom: 0;
  right: 0;
  margin: auto;
  .line-1,
  .line-2,
  .line-3 {
    position: absolute;
    width: 100%;
    height: 2px;
    left: -2px;
    border-radius: 15px;
    transition: all 320ms cubic-bezier(0.42, 0, 0.38, 1.54);
  }
}
.logo {
  height: 50px;
  display: flex;
  width: 100%;
  position: absolute;
  top: 25px;
  left: 0;
  text-align: center;
  .logo_bg {
    background-image: url("../../assets/images/logo.png");
    background-size: 80px;
    background-repeat: no-repeat;
    background-position: center;
    height: 50px;
    display: inline-flex;
    width: 100%;
    position: absolute;
    top: 25px;
    left: 0;
  }
}
.fixed-top {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1030;
}
nav.main-nav {
  border-right: 1px solid #eee;
  background-color: #fff;
  width: 220px;
  display: block;
  position: fixed;
  height: 100vh;
  transition: all 340ms ease-in-out;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.nav-wrapper {
  display: flex;
  position: absolute;
  top: 50% !important;
  left: 50%;
  transform: translate(-50%, -50%);
  flex-basis: 100%;
  align-items: center;
  height: 100%;
}
ul.navigation {
  display: block;
  box-shadow: -3px 5px 12px #f1f1f1;
  width: 110px;
  margin-left: auto !important;
  flex-direction: row;
  li {
    margin: 16px 0;
    text-align: center;
    border-bottom: 1px solid #eee;
    padding-bottom: 10px;
    &:last-child {
      margin-bottom: 0;
    }
    &:hover {
      border-bottom: 1px solid rgb(85, 174, 161);
    }
    a {
      font-size: 14px;
      color: #333;
      i {
        display: block !important;
        padding-bottom: 6px;
        font-size: 16px;
      }
    }
  }
}
.social-media {
  position: absolute;
  bottom: 20px;
  left: 0;
  right: 0;
  text-align: center;
  li {
    display: inline-flex;
  }
  a {
    color: #333;
    font-size: 14px;
    padding-right: 12px;
    transition: all 340ms ease-in-out;
  }
}
.thin {
  font-size: 0.8rem;
  text-align: center;
}
</style>