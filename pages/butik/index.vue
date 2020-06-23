<template>
    <div class="butik-page">
        <Header />
        <div class="butik-full">
            <div class="container">
                <div class="row">
                    <div class="col-md-12">
                        <Breadcrumb />
                    </div>
                    <butik-info />
                    <div class="col-md-8">
                        <div class="b-main-info">
                            <butik-menu />
                        </div>
                        <div class="b-slider">
                            <div class="swiper-btn swiper-button-prev" slot="button-prev">
                                <i class="fas fa-chevron-left"></i>
                            </div>
                            <div class="swiper-btn swiper-button-next" slot="button-next">
                                <i class="fas fa-chevron-right"></i>
                            </div>
                            <no-ssr>
                                <swiper class="bt-slider" :options="swiperOption">
                                    <swiper-slide>
                                        <img :src="require('~/static/butik/bfl1.jpg')" />
                                    </swiper-slide>
                                    <swiper-slide>
                                        <img :src="require('~/static/butik/bfl2.jpg')" />
                                    </swiper-slide>
                                    <swiper-slide>
                                        <img :src="require('~/static/butik/bfl3.jpg')" />
                                    </swiper-slide>
                                </swiper>
                            </no-ssr>
                        </div>
                        <div class="b-news">
                            <div class="row">
                                <div class="col-md-12">
                                    <h4 class="b-sect-title">Свежие новости</h4>
                                </div>
                                <div class="col-md-4">
                                    <div class="article-teas">
                                        <a href="#">
                                            <div class="art-img">
                                                <img :src="require('~/static/article/article4.jpg')" />
                                                <div class="stat">
                                                    <div class="itm">
                                                        <i class="fas fa-eye"></i> 123
                                                    </div>
                                                    <div>
                                                        5 апреля 2019
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="inf">
                                                <div class="title">
                                                    Весенняя акция
                                                </div>
                                                <div class="desc">
                                                    Равным образом постоянный количественный рост и сфера нашей активности играет важную роль
                                                </div>
                                            </div>
                                        </a>
                                    </div>
                                </div>
                                <div class="col-md-4">
                                    <div class="article-teas">
                                        <a href="#">
                                            <div class="art-img">
                                                <img :src="require('~/static/article/article5.jpg')" />
                                                <div class="stat">
                                                    <div class="itm">
                                                        <i class="fas fa-eye"></i> 123
                                                    </div>
                                                    <div>
                                                        24 апреля 2019
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="inf">
                                                <div class="title">
                                                    Рассрочка на ВСЕ категории товаров!
                                                </div>
                                                <div class="desc">
                                                    Равным образом постоянный количественный рост и сфера нашей активности играет важную роль
                                                </div>
                                            </div>
                                        </a>
                                    </div>
                                </div>
                                <div class="col-md-4">
                                    <div class="article-teas">
                                        <a href="#">
                                            <div class="art-img">
                                                <img :src="require('~/static/article/article6.jpg')" />
                                                <div class="stat">
                                                    <div class="itm">
                                                        <i class="fas fa-eye"></i> 123
                                                    </div>
                                                    <div>
                                                        5 апреля 2019
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="inf">
                                                <div class="title">
                                                    Весенняя акция
                                                </div>
                                                <div class="desc">
                                                    Равным образом постоянный количественный рост и сфера нашей активности играет важную роль
                                                </div>
                                            </div>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="b-cat">
                            <div class="row">
                                <div class="col-md-12">
                                    <h4 class="b-sect-title">Популярные</h4>
                                </div>
                                <div class="col-md-12">
                                    <Popular />
                                </div>
                            </div>
                        </div>
                        <div class="b-cat">
                            <div class="row">
                                <div class="col-md-12">
                                    <h4 class="b-sect-title">Новинки</h4>
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Женская зимняя куртка" price="8 200" image="prod7.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod color="black" title="Китайская курта" price="600" image="prod8.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Кеды Nike" price="4 500" image="prod2.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Пуховик" price="2 600" image="prod3.jpg" />
                                </div>
                                <div class="prod-col col-md-4">
                                    <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                </div>
                                <div class="col-all col-md-12">
                                    <nuxt-link to="/butik/catalog"><span>Весь каталог</span><i class="fas fa-chevron-right"></i></nuxt-link>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <Footer />
    </div>
</template>

<script>
import Header from '~/components/Header'
import Breadcrumb from '~/components/Breadcrumb'
import Prod from '~/components/Prod'
import Footer from '~/components/Footer'
import Popular from '~/components/ButPopulat'
import ButikInfo from '~/components/Butikinfo'
import ButikMenu from '~/components/ButikMenu'
export default {
  data () {
    return {
       swiperOption: {
          slidesPerView: 'auto',
          spaceBetween: 0,
          centeredSlides: true,
          loop:true,
          //mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
          },
          speed: 1000,
          autoplay: {
            delay: 5000,
            disableOnInteraction: false
          }
        }
    }
  },
  components: {
    Header,
    Breadcrumb,
    Prod: Prod,
    Footer,
    Popular,
    ButikInfo: ButikInfo,
    ButikMenu: ButikMenu
  },
  methods: {

  },
  mounted () {
    

  }
}
</script>