<template>
  <section class="pricing-one" id="courses">
    <div class="container">
      <div class="block-title text-center">
        <h2 class="block-title__title black-text-color">
          音樂課程內容
        </h2>
        <!-- /.block-title__title -->
      </div>
      <!-- /.block-title -->
      <div class="row">
        <img src="/images/box4.png" />
        <img src="/images/box5.png" />
        <img src="/images/box6.png" />
        <img src="/images/box7.png" />
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </section>
</template>

<script>
export default {
  name: 'Pricing',
};
</script>

<style scoped>
#pricing {
  height: 5400px;
}

.row {
  display: flex;
  justify-content: center;
}

img {
  z-index: 20;
}
</style>
