<template>
    <div class="b1">
      <div class="header-container container">
        <b-row>
          <b-col md="3" cols="6">
            <b-img
              
              class="logo-svg"
              src="~/assets/images/logo-full.svg"
            ></b-img>
          </b-col>
          <b-col md="9" cols="6">
            <div id="dropdown-1">
              <b-dropdown class="m-md-2">
                <template slot="button-content">
                  <b-icon icon="list" class="rounded text-primary p-1"></b-icon>
                </template>
                <b-dropdown-item href="https://esfahanahan.com/"
                  >خانه</b-dropdown-item
                >
                <b-dropdown-item href="#features">امکانات</b-dropdown-item>
                <b-dropdown-item href="#guid-use"
                  >آموزش استفاده</b-dropdown-item
                >
                <b-dropdown-item
                  href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
                  >درباره ما</b-dropdown-item
                >
                <b-dropdown-item
                  href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
                >
                  تماس با ما</b-dropdown-item
                >
              </b-dropdown>
            </div>
            <b-nav id="nav-1" align="end">
              <b-nav-item class="home-link" href="https://esfahanahan.com/"
                >خانه</b-nav-item
              >
              <b-nav-item href="#features">امکانات</b-nav-item>
              <b-nav-item href="#guid-use">آموزش استفاده</b-nav-item>
              <b-nav-item
                href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
                >درباره ما</b-nav-item
              >
              <b-nav-item
                href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
                >تماس با ما</b-nav-item
              >
            </b-nav>
          </b-col>
        </b-row>
      </div>
      <div class="banner-area header-container container">
        <b-row>
          <b-col lg="5" class="mobile-row">
            <b-img left src="~/assets/images/banner.png"> </b-img>
          </b-col>
          <b-col lg="7" class="text-white text-box">
            <b-row class="b-row">
              <h1>معرفی امکان پرداخت سریع موبایلی</h1>
                <h6>
                  مجموعه اصفهان آهن به منظور سهولت در پرداخت صورت حساب مشتریان
                  خود اقدام به راه اندازی سیستم پرداخت موبایلی از طریق کد USSD
                  نموده است . در ادامه به معرفی مزایای این روش و آموزش استفاده
                  از آن میپردازیم.
                </h6>
                <b-container class="mt-5">
                  <b-button  href="#features" class="btn" pill variant="outline-light"
                    >امکانات</b-button
                  >
                  <b-button  href="#features" class="btn" pill variant="outline-light"
                    >آموزش استفاده</b-button
                  >
                </b-container>
            </b-row>
          </b-col>
        </b-row>
      </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      tag: 'reza',
    }
  },
}
</script>

<style lang="scss">
:root {
  direction: rtl;
}
.b1 {
  margin: 0;
  padding: 12px 0 170px 0;
  position: relative;
  z-index: 1;
  overflow: hidden;
  background: linear-gradient(to top right, #181156 40%, #fff 100%);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  &:before {
    content: '';
    top: -35px;
    left: 0;
    right: -35px;
    bottom: 0;
    background-image: url(~/assets/images/header-shape.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    z-index: -1;
    position: absolute;
  }
}
.banner-area{
  margin-top: 70px !important;
}
.header-container {
  margin: 0 400px;
  padding-top: 18px;
  max-width: 100%;
}

a {
  font-size: 14px !important;
  color: white;
  padding: 8px !important;
}

h1 {
  font-size: 35px;
  font-weight: 400 !important;
}
h6 {
  margin-top: 45px;
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
}
.text-box {
  direction: rtl;
  text-align: right;
}
.home-link {
  a {
    color: black;
  }
}
.btn {
  padding: 5px 20px;
  margin: 0 5px;
  font-weight: bold;
}
.b-row {
  font-size: 14px !important;
  padding-top: 140px;
}
#dropdown-1 {
  display: none;
}
@media only screen and (max-width: 994px) {
  .container {
    flex-direction: column;
    justify-content: center !important;
    
    .img-banner {
      max-width: 100%;
    }
  }

  .text-box {
    padding: 0 50px;
  }
  .header-container {
    margin: unset;
    padding-top: unset;
  }
  .row {
    justify-content: center;
    padding: unset !important;
    width: inherit ;
    margin: unset !important;
  }
  h1 {
    font-size: 25px;
    font-weight: 600 !important;
  }
  .mobile-row{
    width: fit-content;
  }
}
@media only screen and (max-width: 768px) {
  #nav-1 {
    display: none;
  }
  #dropdown-1 {
    display: block;
    ul {
      position: absolute;
      background: linear-gradient(
        to right,
        #609eea 0%,
        #47b7e4 42%,
        #21dfdb 85%,
        #1ae7da 100%
      );
      right: -55px;
      top: 100%;
      z-index: 9;
      border: 2px solid white;
      li {
        a {
          color: white;

          text-align: right;
        }
      }
    }
    button {
      padding: 0 5px;
      background-color: black;
      border-radius: 5px;
      height: 28px;
      &:after {
        border: none;
      }
      svg {
        display: block;
        color: white !important;
        margin: 0 auto;
        font-size: 180%;
      }
    }
  }
  .logo-svg {
    width: 100px;
    height: 28.5px;
  }
}
img {
  float: right;
  max-width: 100%;
  height: auto;
}
@media (min-width: 1200px){
  .container {
    
    max-width: 1140px;}
}
.container{
  width: 100% !important;
}

</style>
