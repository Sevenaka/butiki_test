<template>
    <div class="rel">
        <div class="cr-btn left swiper-button-prev5" slot="button-prev">
            <i class="fas fa-chevron-left"></i>
        </div>
        <div class="cr-btn right swiper-button-next5" slot="button-next">
            <i class="fas fa-chevron-right"></i>
        </div>
        <no-ssr>
            <swiper class="prod-slider" :options="swiperOption">
                <swiper-slide>
                    <Prod title="Подарочный набор" price="1 000" image="prod11.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Подарочный набор" price="4 500" image="prod12.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Конфеты" price="2 600" image="prod13.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="Chanel" price="1 300" image="prod14.jpg" />
                </swiper-slide>
                <swiper-slide>
                    <Prod title="COCO Chanel" price="900" image="prod15.jpg" />
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
            nextEl: '.swiper-button-next5',
            prevEl: '.swiper-button-prev5'
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

<style>
.special-bg{
    background: #f9f9f9;
    position: relative;
}
.special{
    position: absolute;
    background-repeat: no-repeat!important;
}
.special-1{
    top:0;
    left: 0;
    background: url('~static/special/special1.jpg');
    width: 224px;
    height: 148px;
}
.special-2{
    bottom: 0;
    left: 0;
    background: url('~static/special/special2.jpg');
    width: 224px;
    height: 112px;
}
.special-3{
    top:0;
    right: 0;
    background: url('~static/special/special3.jpg');
    width: 198px;
    height: 121px;
}
.special-4{
    bottom: 0;
    right: 0;
    background: url('~static/special/special4.jpg');
    width: 198px;
    height: 143px;
}
</style>