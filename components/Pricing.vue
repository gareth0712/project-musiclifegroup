<template>
  <section class="pricing-one" id="pricing">
    <div class="container">
      <div class="block-title text-center">
        <h2 class="block-title__title black-text-color">
          音樂課程內容
        </h2>
        <!-- /.block-title__title -->
      </div>
      <!-- /.block-title -->
      <div class="row">
        <img src="/images/box1.png" />
        <img src="/images/box2.png" />
        <img src="/images/box3.png" />
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </section>
</template>

<script>
export default {
  name: "Pricing",
};
</script>

<style scoped>
#pricing {
  height: 5400px;
}

.row {
  display: flex;
}

img {
  z-index: 20;
}
</style>
