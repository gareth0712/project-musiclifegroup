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
              <a href="#home">主頁</a>
            </li>
            <li class="scrollToLink">
              <a href="#services">服務範疇</a>
            </li>
            <li class="scrollToLink">
              <a href="#brand">品牌概念</a>
            </li>
            <li class="scrollToLink">
              <a href="#contact">聯絡我們</a>
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
