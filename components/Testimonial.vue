<template>
  <section class="testimonials-one" id="testimonials">
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="testimonials-one__image-block swiper-container">
            <div class="swiper-wrapper" id="sync2">
              <swiper :options="swiperOptionsVerticle">
                <swiper-slide>
              <div class="item clearfix">
                <div class="testimonials-one__image">
                  <img src="/images/testi-1-1.jpg" class="testimonials-one__thumb" alt="Awesome Image" />
                  <div class="testimonials-one__qoute">
                    <img src="/images/testi-qoute-1-1.png" alt="Awesome Image" />
                  </div><!-- /.testimonials-one__qoute -->
                </div><!-- /.testimonials-one__image -->
              </div><!-- /.item -->
                </swiper-slide>
                <swiper-slide>
              <div class="item clearfix">
                <div class="testimonials-one__image">
                  <img src="/images/testi-1-2.jpg" class="testimonials-one__thumb" alt="Awesome Image" />
                  <div class="testimonials-one__qoute">
                    <img src="/images/testi-qoute-1-1.png" alt="Awesome Image" />
                  </div><!-- /.testimonials-one__qoute -->
                </div><!-- /.testimonials-one__image -->
              </div><!-- /.item -->
                </swiper-slide>
                <swiper-slide>
              <div class="item clearfix">
                <div class="testimonials-one__image">
                  <img src="/images/testi-1-3.jpg" class="testimonials-one__thumb" alt="Awesome Image" />
                  <div class="testimonials-one__qoute">
                    <img src="/images/testi-qoute-1-1.png" alt="Awesome Image" />
                  </div><!-- /.testimonials-one__qoute -->
                </div><!-- /.testimonials-one__image -->
              </div><!-- /.item -->
                </swiper-slide>
              </swiper>
            </div><!-- /.owl-carousel owl-theme -->
          </div><!-- /.testimonials-one__image-block -->
        </div><!-- /.col-lg-6 -->
        <div class="col-lg-6">
          <div class="testimonials-one__content">
            <div class="block-title text-left">
              <h2 class="block-title__title light-text-color">What our clients <br> are saying</h2><!-- /.block-title__title -->
            </div><!-- /.block-title -->
            <div class="swiper-wrapper" id="sync1">
              <swiper :options="swiperOptions">
                <swiper-slide>
              <div class="item">
                <div class="testimonials-one__single" data-thumb-img="images/testi-1-1.jpg">
                  <p class="testimonials-one__text">This is due to their excellent service, competitive pricing and customer support. It’s throughly refresing to get such a personal touch. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum eu fugiat nulla pariatur.</p><!-- /.testimonials-one__text -->
                  <div class="testimonials-one__bottom">
                    <h3 class="testimonials-one__title">Jona Leisey</h3><!-- /.testimonials-one__title -->
                    <div class="testimonials-one__sep">.</div><!-- /.testimonials-one__sep -->
                    <p class="testimonials-one__designation">CEO Lums</p><!-- /.testimonials-one__designation -->
                  </div><!-- /.testimonials-one__bottom -->
                </div><!-- /.testimonials-one__single -->
              </div><!-- /.item -->
                </swiper-slide>
                <swiper-slide>
              <div class="item">
                <div class="testimonials-one__single" data-thumb-img="images/testi-1-2.jpg">
                  <p class="testimonials-one__text">This is due to their excellent service, competitive pricing and customer support. It’s throughly refresing to get such a personal touch. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum eu fugiat nulla pariatur.</p><!-- /.testimonials-one__text -->
                  <div class="testimonials-one__bottom">
                    <h3 class="testimonials-one__title">Chas Samul</h3><!-- /.testimonials-one__title -->
                    <div class="testimonials-one__sep">.</div><!-- /.testimonials-one__sep -->
                    <p class="testimonials-one__designation">CEO Lums</p><!-- /.testimonials-one__designation -->
                  </div><!-- /.testimonials-one__bottom -->
                </div><!-- /.testimonials-one__single -->
              </div><!-- /.item -->
                </swiper-slide>
                <swiper-slide>
              <div class="item">
                <div class="testimonials-one__single" data-thumb-img="images/testi-1-3.jpg">
                  <p class="testimonials-one__text">This is due to their excellent service, competitive pricing and customer support. It’s throughly refresing to get such a personal touch. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum eu fugiat nulla pariatur.</p><!-- /.testimonials-one__text -->
                  <div class="testimonials-one__bottom">
                    <h3 class="testimonials-one__title">Chelsey Pozar</h3><!-- /.testimonials-one__title -->
                    <div class="testimonials-one__sep">.</div><!-- /.testimonials-one__sep -->
                    <p class="testimonials-one__designation">CEO Lums</p><!-- /.testimonials-one__designation -->
                  </div><!-- /.testimonials-one__bottom -->
                </div><!-- /.testimonials-one__single -->
              </div><!-- /.item -->
                </swiper-slide>
              </swiper>
            </div><!-- /.owl-carousel owl-theme -->
          </div><!-- /.testimonials-one__content -->
        </div><!-- /.col-lg-6 -->
      </div><!-- /.row -->
    </div><!-- /.container -->
  </section>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper'
  import 'swiper/css/swiper.css'

  export default {
    name: "Testimonial",
    components: {
      Swiper,
      SwiperSlide
    },
    directives: {
      swiper: directive
    },
    data() {
      return {
        swiperOptions: {
          slidesPerView : 1,
          loop: true,
          speed: 1000,
          spaceBetween : 30,
          autoplay: {
            delay: 3000,
            disableOnInteraction: false
          },
          pagination: {
            el: '.swiper-pagination',
            type: 'bullets',
            clickable: true
          },
        },

        swiperOptionsVerticle: {
          direction: 'vertical',
          autoplay: {
            delay: 3000,
            disableOnInteraction: false
          },
          pagination: {
            el: '.swiper-pagination',
            clickable: true
          },
        }
      }
    },
  }
</script>

<style scoped>
  .testimonials-one__image-block.swiper-container {
    height: 500px;
  }
</style>
