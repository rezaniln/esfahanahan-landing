<template>
  <div class="d2" @scroll="handleScroll">
    <transition name="fade">
      <div v-show="scY > 300" class="img2" id="pagetop" @click="toTop">
       <p> &#8593;</p>
      </div>
    </transition>
    <div class="img1">
      <img
        ref=""
        src="~/assets/images/5f4612fda3acf607e822f585ac7j.png"
        alt=""
      />
    </div>
    <b-row class="pl-5 pr-5 mr-0 ml-0">
      <b-col xl="6" md="12">
        <p>کلیه حقوق این وبسایت متعلق به شرکت اصفهان آهن آپادانا می باشد</p>
      </b-col>
      <b-col xl="6" md="12">
        <b-nav class="footer-menue">
          <b-nav-item href="https://esfahanahan.com/">خانه</b-nav-item>
          <b-nav-item href="https://esfahanahan.com/landing/ussd/#andriod"
            >ورژن اندروید</b-nav-item
          >
          <b-nav-item href="https://esfahanahan.com/landing/ussd/#ios">
            ورژن IOS</b-nav-item
          >
          <b-nav-item
            href="https://esfahanahan.com/%D8%AF%D8%B1%D8%A8%D8%A7%D8%B1%D9%87-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
          >
            درباره ما</b-nav-item
          >
          <b-nav-item
            href="https://esfahanahan.com/%D8%AA%D9%85%D8%A7%D8%B3-%D8%A8%D8%A7-%D8%A7%D8%B5%D9%81%D9%87%D8%A7%D9%86-%D8%A2%D9%87%D9%86/"
            >تماس با ما</b-nav-item
          >
        </b-nav>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scTimer: 0,
      scY: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      if (this.scTimer) return
      this.scTimer = setTimeout(() => {
        this.scY = window.scrollY
        clearTimeout(this.scTimer)
        this.scTimer = 0
      }, 100)
    },
    toTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth',
      })
    },
  },
}
</script>

<style lang="scss">
.scrolltotop {
    position: fixed;
    bottom: 120px;
    text-align: center;
    right: 30px;
    width: 50px;
    height: 50px;
    z-index: 1000;
    display: none;
    text-decoration: none;
    border-radius: 100%;
    color: #fff;
    font-size: 28px;
    line-height: 48px;
    border: 3px double #fff;
    background: #181156;
    background: linear-gradient(to right, #181156 0%,#50498d 42%,#706ba4 85%,#645f93 100%);
}
.footer-menue {
  justify-content: center;
}
.d2 {
  direction: rtl;
  background: linear-gradient(
    to right,
    #181156 0%,
    #50498d 42%,
    #706ba4 85%,
    #645f93 100%
  );
}
p {
  text-align: center;
  padding-top: 6px;
  color: rgb(255, 255, 255);
}
a {
  color: white;
  &:hover {
    color: black;
  }
}
@media only screen and (max-width: 767px) {
  p {
    font-size: 12px;
  }
  a {
    font-size: 12px !important;
  }
}
.img1 {
  position: fixed;
  width: 70px;
  bottom: 70px;
  z-index: 10;
  img {
    border-radius: 50% !important;
  }
}
.img2 {
  cursor: pointer;
  border-radius: 50%;
  width: 50px;
  position: fixed;
  border: 1px solid rgb(0, 0, 0);
  bottom: 150px;
  right: 10px;
  z-index: 11;
   background: #181156;
    background: linear-gradient(to right, #181156 0%,#50498d 42%,#706ba4 85%,#645f93 100%);
    p{
      font-weight: bolder;
      color: white;
    }
}
</style>
