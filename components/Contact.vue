<template>
  <section class="cta-one" id="contact">
    <div class="container text-center ">
      <div class="block-title">
        <h2 class="block-title__title light-text-color">聯絡我們</h2>
        <!-- /.block-title__title -->
      </div>
      <!-- /.block-title -->
      <a
        :href="whatsappLink"
        class="thm-btn cta-one__btn first-button"
        target="_blank"
        >Whatsapp</a
      >
      <a :href="facebookLink" class="thm-btn cta-one__btn" target="_blank"
        >Facebook</a
      >
    </div>
    <!-- /.container -->
  </section>
</template>

<script>
export default {
  name: "CallToAction",
  data() {
    return {
      whatsappLink:
        "https://api.whatsapp.com/send?phone=85264160526&app=facebook&entry_point=page_cta&fbclid=IwAR155hKk6PZq-9X0jaivk57VMwjiRSJCj02Ej2IhHozW_Pkr2X9oVf56gM8",
      facebookLink:
        "https://www.facebook.com/生命之樂-Music-Life-Group-101231378718871/",
    };
  },
};
</script>

<style scoped>
.first-button {
  margin-right: 12px;
}
</style>
