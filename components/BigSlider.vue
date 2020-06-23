<template>
    <div class="big-sld">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <no-ssr>
                        <swiper class="top-slider" :options="swiperOption">
                            <swiper-slide>
                                <a class="bg-sl-lnk" href="#">
                                    <img :src="require('~/static/big/big.jpg')" />
                                </a>
                            </swiper-slide>
                            <swiper-slide>
                                <a class="bg-sl-lnk" href="#">
                                    <img :src="require('~/static/big/big2.jpg')" />
                                </a>
                            </swiper-slide>
                            <swiper-slide>
                                <a class="bg-sl-lnk" href="#">
                                    <img :src="require('~/static/big/big3.jpg')" />
                                </a>
                            </swiper-slide>
                        </swiper>
                    </no-ssr>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
        swiperOption: {
          slidesPerView: 'auto',
          spaceBetween: 0,
          centeredSlides: true,
          loop:true,
          //mousewheel: true,
          //navigation: {
          //  nextEl: '.swiper-button-next-brand',
          //  prevEl: '.swiper-button-prev-brand'
         // },
          speed: 1000,
          autoplay: {
            delay: 5000,
            disableOnInteraction: false
          }
        }
    }
  },
}
</script>

<style>
.big-sld{
    padding-bottom: 30px;
    overflow: hidden;
}
.top-slider{
    overflow: initial!important;
}
.top-slider .swiper-slide{
    -webkit-transition: all 0.3s ease-out;
    -moz-transition: all 0.3s ease-out;
    -o-transition: all 0.3s ease-out;
    transition: all 0.3s ease-out;
    opacity: 0.5;
    transform: scale(0.9);
}
.top-slider .swiper-slide img{
    border-radius: 5px;
}
.top-slider .swiper-slide-active{
    opacity: 1;
   transform: scale(1);
   z-index: 50;
}
.top-slider .swiper-slide.swiper-slide-prev{
    transform: scale(0.8) translate(200px,0px);
}
.top-slider .swiper-slide.swiper-slide-next{
    transform: scale(0.8) translate(-200px,0px);
}
</style>