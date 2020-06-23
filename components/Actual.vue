<template>
    <div class="rel">
        <div class="cr-btn left swiper-button-prev2" slot="button-prev">
            <i class="fas fa-chevron-left"></i>
        </div>
        <div class="cr-btn right swiper-button-next2" slot="button-next">
            <i class="fas fa-chevron-right"></i>
        </div>
        <no-ssr>
            <swiper class="actual-slider" :options="swiperOption">
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual1.png" />
                        </div>
                        <label>Толстовки</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual2.png" />
                        </div>
                        <label>Футболки</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual3.png" />
                        </div>
                        <label>Куртки</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual4.png" />
                        </div>
                        <label>Все из кожи</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual5.png" />
                        </div>
                        <label>Кеды</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual6.png" />
                        </div>
                        <label>Тулфи</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual7.png" />
                        </div>
                        <label>Пальто</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual8.png" />
                        </div>
                        <label>Зонты</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual9.png" />
                        </div>
                        <label>Шарфы</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual10.png" />
                        </div>
                        <label>Кросовки</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual11.png" />
                        </div>
                        <label>Пиджаки</label>
                    </a>
                </swiper-slide>
                <swiper-slide>
                    <a href="#">
                        <div class="img">
                            <img src="~/static/actual12.png" />
                        </div>
                        <label>Красота</label>
                    </a>
                </swiper-slide>
            </swiper>
        </no-ssr>
    </div>
</template>

<script>
export default {
  data () {
    return {
        swiperOption: {
          slidesPerView: 7,
          spaceBetween: 20,
          //mousewheel: true,
          navigation: {
            nextEl: '.swiper-button-next2',
            prevEl: '.swiper-button-prev2'
          },
        }
    }
  },
  methods: {

  },
  mounted () {
    
  }
}
</script>

<style>
.actual-slider{
    text-align: center;
}
.actual-slider img{
    max-width: 140px;
    max-height: 160px;
}
.actual-slider .img{
    min-height: 180px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.actual-slider a{
    display: block;
    color: #777;
}
.actual-slider a:hover{
    color: #ff280c;
}
.actual-slider label{
    display: block;
    margin-top: 15px;
    font-size: 18px;
    font-weight: 300;
}
</style>