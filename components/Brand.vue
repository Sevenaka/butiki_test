<template>
    <div class="brands">
        <div class="row">
            <div class="col-md-4 z-in">
                <div class="fix-dv">
                    <h3 class="brand-title">Популярные бренды</h3>
                    <div class="brand-al">
                        <a href="#">Смотреть все</a>
                    </div>
                </div>
            </div>
            <div class="col-md-8 rel">
                <div class="cr-btn left swiper-button-prev-brand" slot="button-prev">
                    <i class="fas fa-chevron-left"></i>
                </div>
                <div class="cr-btn right swiper-button-next-brand" slot="button-next">
                    <i class="fas fa-chevron-right"></i>
                </div>
                <no-ssr>
                    <swiper class="brand-slider" :options="swiperOption">
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b1.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b2.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b3.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b4.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b5.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b6.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b7.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b8.jpg')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b9.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b10.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b11.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b12.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b13.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b14.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b15.png')" />
                            </a>
                        </swiper-slide>
                        <swiper-slide>
                            <a class="brand-logo" href="#">
                                <img :src="require('~/static/brand/b16.png')" />
                            </a>
                        </swiper-slide>
                    </swiper>
                </no-ssr>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
        swiperOption: {
          slidesPerView: 9,
          spaceBetween: 20,
          mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next-brand',
            prevEl: '.swiper-button-prev-brand'
          }
        }
    }
  },
}
</script>

<style>
.brand-bg{
    background: #fdf1ec;
    overflow: hidden;
    position: relative;
}
.brand-title{
    margin-bottom: 0px;
    font-size: 34px;
}
.fix-dv{
    display: flex;
    align-content: center;
    height: 100%;
    align-items: end;
    position: relative;
    flex-wrap: wrap;
    flex-flow: column;
    justify-content: center;
}
.fix-dv::after{
    content: "";
    position: absolute;
    background: #fdf1ec;
    z-index: -1;
    top:-50px;
    bottom: -50px;
    right: 0;
    left: -3000px;
}
.brand-logo{
    display: block;
    background: white;
    width: 90px;
    height: 90px;
    border-radius: 50%;
    overflow: hidden;
    text-align: center;
    line-height: 90px;
    transition: all 0.2s ease-out;
}
.brand-logo:hover{
    -webkit-transform: scale(0.9);
    transform: scale(0.9);
}
.brand-logo img{
    width: 100%;
    max-width: 70px;
}
.brand-slider{
    overflow: initial!important;
}
.z-in{
    position: relative;
    z-index: 20;
}
.brand-bg::after{
    content: "";
    position: absolute;
    z-index: 10;
    top:0;
    bottom: 0;
    right: 0;
    width: 200px;
    background: -moz-linear-gradient(left, rgba(255,255,255,0) 0%, rgba(253,242,237,1) 96%, rgba(253,241,236,1) 100%); /* FF3.6-15 */
    background: -webkit-linear-gradient(left, rgba(255,255,255,0) 0%,rgba(253,242,237,1) 96%,rgba(253,241,236,1) 100%); /* Chrome10-25,Safari5.1-6 */
    background: linear-gradient(to right, rgba(255,255,255,0) 0%,rgba(253,242,237,1) 96%,rgba(253,241,236,1) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00ffffff', endColorstr='#fdf1ec',GradientType=1 ); /* IE6-9 */
}
.swiper-button-prev-brand{
    left: -60px!important;
}
.brand-al{
    margin-top: 3px;
}
.brand-al a{
    border-bottom: 1px solid;
    color: #ff280c;
    font-weight: bold;
}
</style>