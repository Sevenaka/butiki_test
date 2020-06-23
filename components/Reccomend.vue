<template>
    <div class="rel">
        <div class="cr-btn left swiper-button-prev4" slot="button-prev">
            <i class="fas fa-chevron-left"></i>
        </div>
        <div class="cr-btn right swiper-button-next4" slot="button-next">
            <i class="fas fa-chevron-right"></i>
        </div>
        <no-ssr>
            <swiper class="prod-slider" :options="swiperOption">
                <swiper-slide>
                    <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Женская зимняя куртка" price="8 200" image="prod7.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod color="black" title="Китайская курта" price="600" image="prod8.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
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
          slidesPerView: 5,
          spaceBetween: 10,
          //mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next4',
            prevEl: '.swiper-button-prev4'
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