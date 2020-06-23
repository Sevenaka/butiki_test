<template>
    <div class="rel">
        <div class="cr-btn left swiper-button-prev3" slot="button-prev">
            <i class="fas fa-chevron-left"></i>
        </div>
        <div class="cr-btn right swiper-button-next3" slot="button-next">
            <i class="fas fa-chevron-right"></i>
        </div>
        <no-ssr>
            <swiper class="prod-slider" :options="swiperOption">
                <swiper-slide>
                    <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Кеды Nike" price="4 500" image="prod2.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Пуховик" price="2 600" image="prod3.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Бальное платье" price="1 300" image="prod4.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Футболка Suprime" price="900" image="prod5.png" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Кеды Nike" price="4 500" image="prod2.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Пуховик" price="2 600" image="prod3.jpg" />
                </swiper-slide>
            </swiper>
        </no-ssr>
    </div>
</template>

<script>
import Prod from '~/components/Prod'
export default {
  data () {
    return {
        swiperOption: {
          slidesPerView: 3,
          spaceBetween: 30,
          //mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next3',
            prevEl: '.swiper-button-prev3'
          },
        }
    }
  },
  components: {
      Prod: Prod
  },
  methods: {

  },
  mounted () {
    
  }
}
</script>