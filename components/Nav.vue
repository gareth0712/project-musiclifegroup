<template>
  <header class="site-header header-one ">
    <nav
      :class="
        `navbar navbar-expand-lg navbar-light header-navigation stricky ${
          sticky ? 'stricked-menu stricky-fixed' : ''
        }`
      "
    >
      <div class="container clearfix">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="logo-box clearfix">
          <a class="navbar-brand" href="/">
            <img
              src="/images/logo-light.png"
              class="main-logo"
              width="66"
              alt="Awesome Image"
            />
          </a>
          <button class="menu-toggler" data-target=".main-navigation">
            <span
              @click="mobileToggle = !mobileToggle"
              class="fa fa-bars"
            ></span>
          </button>
        </div>
        <!-- /.logo-box -->
        <!-- Collect the nav links, forms, and other content for toggling -->
        <div
          :class="`main-navigation ${mobileToggle ? 'showen' : ''}`"
          :style="`display: ${mobileToggle ? 'block' : 'none'}`"
        >
          <ul class=" navigation-box one-page-scroll-menu ">
            <li class="current scrollToLink">
              <a href="#home">關於我們</a>
            </li>
            <li class="scrollToLink">
              <a href="#services">Features</a>
            </li>
            <li class="scrollToLink">
              <a href="#pricing">Pricing</a>
            </li>
            <li class="scrollToLink">
              <a href="#testimonials">Testimonials</a>
            </li>
            <li class="scrollToLink">
              <a href="#blog">Blog</a>
              <ul class="sub-menu" style="display: block">
                <li><nuxt-link to="/blog">Blog</nuxt-link></li>
                <li><nuxt-link to="/blog-details">Blog Details</nuxt-link></li>
              </ul>
              <!-- /.sub-menu -->
            </li>
            <li class="scrollToLink">
              <a href="#contact">Contact</a>
            </li>
          </ul>
        </div>
        <!-- /.navbar-collapse -->
        <div class="right-side-box">
          <a href="#" class="thm-btn header-one__btn">Contact</a>
        </div>
        <!-- /.right-side-box -->
      </div>
      <!-- /.container -->
    </nav>
  </header>
</template>

<script>
export default {
  name: "Nav",
  data() {
    return {
      sticky: false,
      mobileToggle: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.scrollY > 70) {
        this.sticky = true;
      } else if (window.scrollY < 70) {
        this.sticky = false;
      }
    },
  },
};
</script>

<style scoped></style>
