<template>
  <section class="banner-one" id="home">
    <span class="banner-one__shape-1"></span>
    <span class="banner-one__shape-2"></span>
    <span class="banner-one__shape-3"></span>
    <span class="banner-one__shape-4"></span>
    <span class="banner-one__shape-5"></span>
    <span class="banner-one__shape-6"></span>

    <img
      src="/images/globe-1-1.png"
      class="banner-one__globe"
      alt="Awesome Image"
    />
    <img
      src="/images/rocket-1-1.png"
      class="banner-one__rocket"
      alt="Awesome Image"
    />
    <!-- <img src="/images/banner.png" class="banner-one__moc" alt="Awesome Image" /> -->
    <div class="container">
      <div class="row">
        <div class="col-xl-6">
          <div class="banner-one__content">
            <!-- /.banner-one__tag-line -->
            <h3 class="banner-one__title">
              Piano Dream
            </h3>
            <!-- /.banner-one__title -->
          </div>
          <!-- /.banner-one__content -->
        </div>
        <!-- /.col-lg-6 -->
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </section>
</template>

<script>
export default {
  name: 'Banner',
};
</script>

<style scoped>
.banner-one__title {
  color: #fff;
}
</style>
