<template>
  <div class="container">
    <b-container class="ussd">
      <b-col cols="12">
        <p class="text p1">*6655*34045#</p>
      </b-col>
    </b-container>
    <b-container>
      <h3>امکانات</h3>
      <h6>
        استفاده از روش پرداخت USSD به وسیله موبایل امکانات زیر را به شما میدهد
      </h6>
    </b-container>
    <b-container>
      <b-row class="icon-card mt-5">
        <b-col md="3">
          <b-card>
            <b-icon icon="lock-fill" class="rounded text-primary p-1"></b-icon>
            <h4>امنیت</h4>
            <h6>بالای پرداخت اینترنتی</h6>
          </b-card>
        </b-col>
        <b-col md="3">
          <b-card>
            <b-icon icon="graph-up" class="rounded text-primary p-1"></b-icon>
            <h4>صرفه جویی</h4>
            <h6>در وقت و هزینه</h6>
          </b-card>
        </b-col>
        <b-col md="3">
          <b-card>
            <b-icon
              icon="clock-history"
              class="rounded text-primary p-1"
            ></b-icon>
            <h4>سرعت</h4>
            <h6>بالا برای پرداخت</h6>
          </b-card>
        </b-col>
        <b-col md="3">
          <b-card>
            <b-icon icon="phone" class="rounded text-primary p-1"></b-icon>
            <h4>دسترسی</h4>
            <h6>ساده در هر کجا</h6>
          </b-card>
        </b-col>
      </b-row>
      <b-row  class="mt-5 data-box">
        <b-col cols="6" class="ul-content"
          >
              <h4>آموزش پرداخت از طریق USSD کد</h4>
            <ul class="ul-content mt-5">
                <li><b>فرایند پرداخت موبایلی اصفهان آهن بسیار ساده است </b></li>
              <li>
                <span> &#8592;</span>
                <span>ابتدا وارد صفحه شماره گیری تلفن همراه خود شوید</span>
              </li>
              <li>
                <span> &#8592; </span>
                <span>سپس کد *6655*34045# را شماره گیری نمایید.</span>
              </li>
              <li>
                <span> &#8592; </span>
                <span>پس از شماره گیری بر روی تماس کلیک کنید.</span>
              </li>
              <li>
                <span> &#8592; </span>
                <span>یکی از دو گزینه پرداخت بیعانه و تسویه حساب را وارد نموده و بر
                  روی ارسال کلیک کنید.</span>
              </li>
              <li>
                <span> &#8592; </span>
                <span
                  >مبلغ مورد نظر را انتخاب یا وارد نموده و بر روی ارسال کلیک
                  کنید.</span
                >
              </li>
              <li>
                <span> &#8592; </span>
                <span
                  >لینک پرداخت اینترنتی برای شما از طریق پیامک ارسال
                  میشود.</span
                >
              </li>
              <li>
                <span> &#8592; </span>
                <span
                  >بر روی لینک داخل پیامک کلیک کنید تا وارد صفحه پرداخت
                  شوید.</span
                >
              </li>
              <li>
                <span> &#8592; </span>
                <span
                  >با تکمیل فرایند خرید اینترنتی پرداخت شما کامل شده است.
                </span>
              </li>
            </ul>
          </b-col>
        <b-col class="video" cols="6"
          ><video controls>
            <source
              src="https://esfahanahan.com/landing/ussd/assets/video/ussd.mp4"
              type="video/mp4"
            />
          </video>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<style lang="scss" scoped>
.p1{
  width: fit-content;
  margin: 0 auto;
  font-size: 150px;
  font-weight: 700;
  color: hsl(220, 46%, 48%/1);
  text-shadow: 1px 1px 1px hsl(220deg, 46%, 38%),
    1px 2px 1px hsl(220deg, 46%, 38%), 1px 3px 1px hsl(220deg, 46%, 38%),
    1px 4px 1px hsl(220deg, 46%, 38%), 1px 5px 1px hsl(220deg, 46%, 38%),
    1px 6px 1px hsl(220deg, 46%, 38%), 1px 7px 1px hsl(220deg, 46%, 38%),
    1px 8px 1px hsl(220deg, 46%, 38%), 1px 9px 1px hsl(220deg, 46%, 38%),
    1px 10px 1px hsl(220deg, 46%, 38%), 1px 18px 6px rgb(60, 60, 60 / 30%),
    1px 22px 10px rgb(60, 60, 60 / 10%), 1px 25px 35px rgb(60, 60, 60 / 10%),
    1px 30px 60px rgb(60, 60, 60 / 30%);
}
h3 {
  margin-top: 50px;
  text-align: center;
}
h6 {
  text-align: center;
  margin-top: 30px;
}
.icon-card {
  text-align: center;
}
svg {
  height: 4em;
  width: 4em;
  margin: 0 auto;
  
}
video {
  width: inherit;
}
.ul-content {
    padding-right: 0px;
  text-align: right;
  list-style-type: none;
  direction: rtl;
}
li{
        span:first-child{
            
            margin-left: 10px;
        }
}
li{
        span:last-child{
          display: inline-block;
          font-size: 12px;
            
        }
}
.container{
  max-width: 1140px;
}
@media (min-width:768px) and (max-width:991px){
  .text{
  font-size:80px
}
}
@media  only screen and (max-width:767px){
   .text{
     font-size: 40px;
   } 
  .data-box{
  flex-direction: column-reverse;
  align-items: center;
  justify-content: center;
    .video {
     max-width: 100%;
    }
    .ul-content{
      max-width: 100%;
    }
  }
  }
  .text{
    direction: ltr;
    text-align: right;
  }
 


</style>
