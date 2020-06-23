<template>
  <div class="wrap">
    <Header />
    <main>

      <BigSlider />

      <!--
      <div class="slide-container">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
                <no-ssr>
                <swiper class="main-cr" :options="swiperOption">
                  <div class="swiper-btn swiper-button-prev" slot="button-prev">
                    <i class="fas fa-chevron-left"></i>
                  </div>
                  <div class="swiper-btn swiper-button-next" slot="button-next">
                    <i class="fas fa-chevron-right"></i>
                  </div>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-1">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Новинки женско одежды</div>
                        <div class="desc">Только лучшие цены</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-2">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Лучшее по сезону</div>
                        <div class="desc">Купите что нибудь</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-3">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Поступление обуви</div>
                        <div class="desc">Кеды, шмеды</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-4">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Новые скидки</div>
                        <div class="desc">Покйпайте с умом</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-5">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Выбор есть всегда</div>
                        <div class="desc">Но не у вас</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-6">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Женские аксессуары</div>
                        <div class="desc">Очки, мачки брат</div>
                      </div>
                    </div>
                  </swiper-slide>
                  <swiper-slide>
                    <div class="cr-slide slide-bg-7">
                      <div class="img"></div>
                      <div class="text">
                        <div class="title">Поступление платьев</div>
                        <div class="desc">Купить платье сука</div>
                      </div>
                    </div>
                  </swiper-slide>
                </swiper>
                </no-ssr>
            </div>
          </div>
        </div>
      </div>
      -->
      <section class="front-sect">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <h2 class="sect-title">Актуальные вещи этой весны</h2>
              <ActualSlider />
            </div>
          </div>
        </div>
      </section>
      <div class="bg-sect">
        <section class="front-sect special-bg">
          <span class="special special-1"></span>
          <span class="special special-2"></span>
          <span class="special special-3"></span>
          <span class="special special-4"></span>
          <div class="container">
            <div class="row">
              <div class="col-md-12">
                <h2 class="sect-title sect-title-ico">
                  <span><img src="~/static/heart.svg">День всех влюбленных</span>
                </h2>
                <Special />
              </div>
            </div>
          </div>
        </section>
        <section class="front-sect">
          <div class="container">
            <div class="row">
              <div class="col-md-12">
                <h2 class="sect-title">Новые поступления</h2>
                <New />
              </div>
            </div>
          </div>
        </section>
        <section class="front-sect">
          <div class="container">
            <div class="row">
              <div class="col-md-12">
                <h2 class="sect-title">Рекомендуем</h2>
                <Reccomend />
              </div>
            </div>
          </div>
        </section>
      </div>
      <section class="front-sect">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <h2 class="sect-title">Взгляните на их товар</h2>
              <ShopProd />
            </div>
          </div>
        </div>
      </section>

      <section class="front-sect brand-bg">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <Brand />
            </div>
          </div>
        </div>
      </section>

      <section class="front-sect">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <h2 class="sect-title">Новости бутиков</h2>
              <News />
            </div>
          </div>
        </div>
      </section>
      <section class="front-sect">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <h2 class="sect-title">Модный блог</h2>
              <Article />
            </div>
          </div>
        </div>
      </section>
      <section class="front-sect arenda-sect">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <Arenda />
            </div>
          </div>
        </div>
      </section>
    </main>
    <Footer />
  </div>
</template>

<script>
import 'swiper/dist/css/swiper.css'

import ActualSlider from '~/components/Actual'
import New from '~/components/New'
import Reccomend from '~/components/Reccomend'
import Special from '~/components/Special'
import ShopProd from '~/components/ShopProd'
import Article from '~/components/Article'
import News from '~/components/News'
import Footer from '~/components/Footer'
import Brand from '~/components/Brand'
import Arenda from '~/components/Arenda'
import BigSlider from '~/components/BigSlider'
import Header from '~/components/Header'

export default {
  data () {
    return {
        swiperOption: {
          slidesPerView: 4,
          spaceBetween: 20,
          loop: true,
          mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
          },
          //autoplay: {
           // delay: 8000,
           // disableOnInteraction: false
          //},
          //pagination: {
          //  el: '.swiper-pagination',
            //clickable: true
          //}
        }
    }
  },
  components: {
    ActualSlider,
    New,
    Reccomend,
    Special,
    ShopProd,
    Article,
    News,
    Footer,
    Brand,
    Arenda,
    BigSlider,
    Header
  },
  methods: {
    actionMenu(){
      this.menuOpen = this.menuOpen == false ? true : false;
      console.log(this.menuOpen);
    },
    mouseoverSubmenu(menu){
      this.subMenu = menu
    }
  },
  mounted () {
    

  }
}
</script>

