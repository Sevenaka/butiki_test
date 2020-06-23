<template>
    <div class="rel">
        <div class="cr-btn left swiper-button-prev7" slot="button-prev">
            <i class="fas fa-chevron-left"></i>
        </div>
        <div class="cr-btn right swiper-button-next7" slot="button-next">
            <i class="fas fa-chevron-right"></i>
        </div>
        <no-ssr>
            <swiper class="prod-slider" :options="swiperOption">
                <swiper-slide>
                    <div class="shop-card">
                        <a href="#">
                            <div class="shop-inf">
                                <img :src="require('~/static/logo/logo2.jpg')" />
                                <h4>SUVARI</h4>
                                <div class="desc">
                                    Бутик женской одежды
                                </div>
                            </div>
                            <div class="shop-list">
                                <div class="row">
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod1.jpg')" />
                                        <div class="title">Женская куртка</div>
                                        <div class="price">1 500 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod7.jpg')" />
                                        <div class="title">Зимняя куртка</div>
                                        <div class="price">16 000 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod3.jpg')" />
                                        <div class="title">Пуховик</div>
                                        <div class="price">94 000 тг.</div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="shop-card">
                        <a href="#">
                            <div class="shop-inf">
                                <img :src="require('~/static/logo/logo1.png')" />
                                <h4>KOTON</h4>
                                <div class="desc">
                                    Магазин женской одежды
                                </div>
                            </div>
                            <div class="shop-list">
                                <div class="row">
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod2.jpg')" />
                                        <div class="title">Кеды Nike</div>
                                        <div class="price">4 500 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod5.png')" />
                                        <div class="title">Футболка</div>
                                        <div class="price">6 000 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod9.jpg')" />
                                        <div class="title">Абибас</div>
                                        <div class="price">4 000 тг.</div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="shop-card">
                        <a href="#">
                            <div class="shop-inf">
                                <img :src="require('~/static/logo/logo3.jpg')" />
                                <h4>PRIMAVERA</h4>
                                <div class="desc">
                                    Бутик женской одежды
                                </div>
                            </div>
                            <div class="shop-list">
                                <div class="row">
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod14.jpg')" />
                                        <div class="title">Chanel</div>
                                        <div class="price">1 500 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod6.jpg')" />
                                        <div class="title">Женская куртка</div>
                                        <div class="price">9 000 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod8.jpg')" />
                                        <div class="title">Куртка</div>
                                        <div class="price">7 800 тг.</div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="shop-card">
                        <a href="#">
                            <div class="shop-inf">
                                <img :src="require('~/static/logo/logo1.png')" />
                                <h4>KOTON</h4>
                                <div class="desc">
                                    Магазин женской одежды
                                </div>
                            </div>
                            <div class="shop-list">
                                <div class="row">
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod2.jpg')" />
                                        <div class="title">Кеды Nike</div>
                                        <div class="price">4 500 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod5.png')" />
                                        <div class="title">Футболка</div>
                                        <div class="price">6 000 тг.</div>
                                    </div>
                                    <div class="col-md-4">
                                        <img :src="require('~/static/prod/prod9.jpg')" />
                                        <div class="title">Абибас</div>
                                        <div class="price">4 000 тг.</div>
                                    </div>
                                </div>
                            </div>
                        </a>
                    </div>
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
          spaceBetween: 20,
          //mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next7',
            prevEl: '.swiper-button-prev7'
          },
        }
    }
  },
  components: {

  },
  methods: {

  },
  mounted () {
    
  }
}
</script>

<style>
.shop-card{
    border: 1px solid rgba(204, 204, 204, 0.33);
    border-radius: 5px;
    padding-top: 30px;
    padding-bottom: 20px;
    padding-left: 15px;
    padding-right: 15px;
}
.shop-card a{
    display: block;
}
.shop-card .shop-inf{
    text-align: center;
}
.shop-card .shop-inf img{
    max-width: 100px;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 1px solid rgba(204, 204, 204, 0.5);
}
.shop-card .shop-inf .desc{
    color: #777;
    font-weight: 300;
}
.shop-card .shop-inf h4{
    color:#222;
    font-size: 20px;
    margin-bottom: 6px;
}
.shop-list{
    margin-top: 20px;
}
.shop-list img{
    width: 100%;
}
.shop-list .title{
    font-size: 13px;
    margin-top: 10px;
    color: #222;
    margin-bottom: 5px;
}
.shop-list .price{
    font-size: 14px;
    color: #777;
}
</style>