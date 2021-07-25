<template>
  <div class="d-container">
    <div class="b1">
        <b-row class="m-4">
          <b-col cols="2">
            <b-img right class="logo-svg" src="../images/logo-full.svg"></b-img>
          </b-col>
          <b-col cols="10">
            <b-nav align="end">
              <b-nav-item class="home-link">خانه</b-nav-item>
              <b-nav-item>امکانات</b-nav-item>
              <b-nav-item>آموزش استفاده</b-nav-item>
              <b-nav-item>درباره ما</b-nav-item>
              <b-nav-item>تماس با ما</b-nav-item>
            </b-nav>
          </b-col>
        </b-row>
        <b-row class="mt-5 mr-0">
          <b-col lg="5">
            <b-img left src="..\images\banner.png"> </b-img>
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
export default {}
</script>

<style lang="scss">
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
    background-image: url(../images/header-shape.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    z-index: -1;
    position: absolute;
    -webkit-box-sizing: border-box;
    width: inherit;
    height: inherit;

    
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
.b-row{
  padding-top: 170px;
}
.d-container{
  direction: rtl;
}
</style>
