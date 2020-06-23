<template>
    <div class="torg-page">
        <Header />
        <div class="torg-full">
            <div class="container">
                <div class="row">
                    <div class="col-md-12">
                        <Breadcrumb />
                    </div>
                    <div class="col-md-4">
                        <div class="c-info-cnt">
                            <div class="img-bg">
                                <div class="tr-inf">
                                    <div class="tr-logo">
                                        <img src="~/static/torgovy/im.svg" />
                                    </div>
                                    <div class="tr-text">
                                        <h1>
                                            <div class="ln2">Император</div> <div class="ln1">Торговый комплекс</div></h1>
                                    </div>
                                </div>
                            </div>
                            <div class="b-sect">
                                <div class="b-field">
                                    <label>Адрес:</label>
                                    <p>Ауэзова проспект, 28</p>
                                    <p><i class="fas fa-map-marker-alt"></i> <span class="aj-lnk">Показать на карте</span></p>
                                </div>
                                <div class="b-field">
                                    <label>Телефоны:</label>
                                    <p>+7 (705) <span class="aj-lnk">Показать телефоны</span></p>
                                </div>
                                <div class="b-field">
                                    <label>Сайт:</label>
                                    <p><a href="https://www.tk-imperator.kz/">https://www.tk-imperator.kz/</a></p>
                                </div>
                                <div class="b-field">
                                    <label>Режим работы:</label>
                                    <div class="rb-map">
                                        <div class="rb-itm">
                                            <div class="r-bg today">
                                                <div class="tt">ПН</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    18:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">ВТ</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    18:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">СР</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    18:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">ЧТ</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    18:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">ПТ</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    18:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">СБ</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    22:00
                                                </div>
                                            </div>
                                        </div>
                                        <div class="rb-itm">
                                            <div class="r-bg">
                                                <div class="tt">ВС</div>
                                                <div class="tm">
                                                    10:00<br/>
                                                    22:00
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-8">
                       Описание
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
import Footer from '~/components/Footer'
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
    Footer,
  },
  methods: {

  },
  mounted () {
    

  }
}
</script>

<style>
.torg-full{
    padding-bottom: 50px;
    padding-top: 30px;
}
.c-info-cnt{
    border: 1px solid rgba(204, 204, 204, 0.5);
    border-radius: 5px;
    padding: 30px;
    overflow: hidden;
    min-height: 500px;
}
.img-bg{
    position: relative;
    background: url('~static/torgovy/torgbg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 250px;
    margin-top: -31px;
    margin-left: -31px;
    margin-right: -31px;
}
.img-bg::after{
    content: "";
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    height: 120px;
    background: linear-gradient(to bottom, rgba(0,0,0,0) 0%,rgba(0,0,0,0.65) 96%,rgba(0,0,0,0.65) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00000000', endColorstr='#a6000000',GradientType=0 );
}
.tr-inf{
    color: white;
    position: absolute;
    left: 15px;
    right: 15px;
    bottom: 15px;
    z-index: 10;
    padding-left: 110px;
}
.tr-logo{
    width: 80px;
    height: 80px;
    display: flex;
    background: white;
    overflow: hidden;
    border-radius: 50%;
    justify-content: center;
    align-items: center;
    position: absolute;
    left: 0;
    bottom: -5px;
}
.tr-logo img{
    max-width: 70px;
}
.tr-inf .tr-text{

}
.tr-inf .tr-text h1{
    
}
.tr-inf .tr-text h1 .ln1{
    font-size: 16px;
}
.tr-inf .tr-text h1 .ln2{
    font-size: 32px;
}
.rb-map{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: -2px;
    margin-right: -2px;
}
.rb-map .rb-itm{
    -ms-flex-preferred-size: 0;
    flex-basis: 0;
    -ms-flex-positive: 1;
    flex-grow: 1;
    max-width: 100%;
    text-align: center;
    padding-left: 2px;
    padding-right: 2px;
}
.rb-map .rb-itm .r-bg{
    padding-bottom: 5px;
    padding-top: 5px;
    border-radius: 3px;
}
.rb-map .rb-itm .r-bg.today{
    background: #2185d0;
    color: white;
}
.rb-map .tm{
    font-size: 14px;
    line-height: 18px;
}
.rb-map .rb-itm .tt{
    font-size: 13px;
    margin-bottom: 8px;
    font-weight: bold;
}
</style>