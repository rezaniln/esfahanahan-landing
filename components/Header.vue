<template>
  <div class="d-container">
    <div class="b1">
      <b-row class="m-4">
        <b-col cols="2">
          <b-img right class="logo-svg" src="~/assets/images/logo-full.svg"></b-img>
        </b-col>
        <b-col cols="10">
          <div id="dropdown-1">
            <b-dropdown   class="m-md-2">
             <template slot="button-content" >
                <b-icon icon="list" class="rounded text-primary p-1"></b-icon>
             </template>
              <b-dropdown-item>خانه</b-dropdown-item>
              <b-dropdown-item>امکانات</b-dropdown-item>
              <b-dropdown-item>آموزش استفاده</b-dropdown-item>
              <b-dropdown-item>درباره ما</b-dropdown-item>
              <b-dropdown-item> تماس با ما</b-dropdown-item>
            </b-dropdown>
          </div>
          <b-nav id="nav-1" align="end">
            <b-nav-item class="home-link">خانه</b-nav-item>
            <b-nav-item>امکانات</b-nav-item>
            <b-nav-item>آموزش استفاده</b-nav-item>
            <b-nav-item>درباره ما</b-nav-item>
            <b-nav-item>تماس با ما</b-nav-item>
          </b-nav>
        </b-col>
      </b-row>
      <b-row class="mt-5 mr-0 flex-container">
        <b-col class="img-banner" lg="5">
          <b-img left src="~/assets/images/banner.png"> </b-img>
        </b-col>
        <b-col lg="5" class="text-white text-box">
          <b-row class="b-row">
            <div>
              <h2>معرفی امکان پرداخت سریع موبایلی</h2>
              <h6>
                مجموعه اصفهان آهن به منظور سهولت در پرداخت صورت حساب مشتریان خود
                اقدام به راه اندازی سیستم پرداخت موبایلی از طریق کد USSD نموده
                است . در ادامه به معرفی مزایای این روش و آموزش استفاده از آن
                میپردازیم.
              </h6>
              <b-container class="mt-5">
                <b-button class="btn" pill variant="outline-light"
                  >امکانات</b-button
                >
                <b-button class="btn" pill variant="outline-light"
                  >آموزش استفاده</b-button
                >
              </b-container>
            </div>
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
      tag:"reza"
    }
  },
}
</script>

<style lang="scss">
:root{
  direction: rtl;
}
.b1 {
  margin: 0;
  padding: 12px 0 170px 0;
  position: relative;
  z-index: 1;
  overflow: hidden;
  background: linear-gradient(to top right, #181156 40%, #fff 100%);
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

a {
  color: white;
}

h1 {
  margin-top: 100px;
}
h6 {
  margin-top: 45px;
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
  padding: 10px 40px;
  margin: 0 10px;
}
.b-row {
  padding-top: 170px;
}
.d-container {
  direction: rtl;
}
#dropdown-1{
  display: none;
}
@media only screen and (max-width: 992px) {
  .flex-container{
    flex-direction: column;
    justify-content: center !important;
    align-items: center !important;
    .img-banner{
      max-width: fit-content;
     
    }
      
  }

.text-box{
  padding:0 50px;
}
}
@media only screen and (max-width: 768px) {
  #nav-1{
    display: none;
  }
    #dropdown-1{
      display: block;
        ul{
          
          position: absolute;
          background:linear-gradient(to right, #609eea 0%,#47b7e4 42%,#21dfdb 85%,#1ae7da 100%);
          right: -55px;
          top: 100%;
          z-index: 9;
          border: 2px solid white;
            li{
              
                a{
                  color: white;
                  
                  text-align: right;
                }
            }
        }
        button{
          padding:0 5px;
          background-color: black;
          border-radius: 5px;
          height: 28px;
           &:after{
            border: none;
          }
            svg{
              display: block;
              color: white !important;
              margin: 0 auto;
              font-size: 180%;
            }
        }
    }
    .logo-svg{
      width: 100px;
      height: 28.5px;
    }

}
</style>
