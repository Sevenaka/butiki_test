<template>
    <div class="arenda-cont">
        <div class="row">
            <div class="col-md-3 z-in">
                <div class="ar-dv">
                    <h3 class="ar-tit">Аренда/Продажа бутиков</h3>
                    <div class="brand-al"><a href="#">Смотреть все</a></div>
                </div>
            </div>
            <div class="col-md-9">
                <no-ssr>
                    <swiper class="arenda-slider" :options="swiperOption">
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>98 000 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Алматы
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 18
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda1.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Бутик площадью 197.2 м²</div>
                                        <div class="addr">Ауэзовский р-н, Джандосова 200В — Саина</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>700 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Алматы
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 123
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda2.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Магазин площадью 1280 м²</div>
                                        <div class="addr">Бостанд р-н, Жарокова 137/1 — Мынбаева</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>40 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Усть-Каменогорск
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 6
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda3.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Магазин площадью 37 м²</div>
                                        <div class="addr">Бостанд р-н, Жарокова 137/1 — Мынбаева</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>98 000 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Алматы
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 18
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda1.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Бутик площадью 197.2 м²</div>
                                        <div class="addr">Ауэзовский р-н, Джандосова 200В — Саина</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>700 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Алматы
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 123
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda2.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Магазин площадью 1280 м²</div>
                                        <div class="addr">Бостанд р-н, Жарокова 137/1 — Мынбаева</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="arenda-ts">
                                <div class="price"><strong>40 000</strong> тг.</div>
                                <a href="#">
                                    <div class="img">
                                        <div class="ar-stat">
                                            <div class="itm">
                                                18 апреля 2019
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-map-marker-alt"></i> Усть-Каменогорск
                                            </div>
                                            <div class="itm">
                                                <i class="fas fa-eye"></i> 6
                                            </div>
                                            <div class="ar-fv"><i class="far fa-heart"></i></div>
                                        </div>
                                        <img :src="require('~/static/arenda/arenda3.jpg')" />
                                    </div>
                                    <div class="inf">
                                        <div class="title">Магазин площадью 37 м²</div>
                                        <div class="addr">Бостанд р-н, Жарокова 137/1 — Мынбаева</div>
                                        <p>
                                            в жилом доме, сигнализация, пожарная сигнализация, видеонаблюдение, круглосуточная охрана, Коммерческое 
                                        </p>
                                    </div>
                                </a>
                            </div>
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
          slidesPerView: 3,
          spaceBetween: 30,
          mousewheel: true,
          //navigation: {
          //  nextEl: '.swiper-button-next-brand',
          //  prevEl: '.swiper-button-prev-brand'
         // },
        }
    }
  },
}
</script>

<style>
.z-in{
    position: relative;
    z-index: 20;
}
.arenda-sect{
    background: #fafafa;
    overflow: hidden;
    border-top: 1px solid #f1f1f1;
    position: relative;
}
.ar-dv{
    display: flex;
    align-content: center;
    height: 100%;
    align-items: end;
    position: relative;
    flex-wrap: wrap;
    flex-flow: column;
    justify-content: center;
}
.ar-dv::after{
    content: "";
    z-index: -1;
    top: -50px;
    bottom: -50px;
    right: 0;
    left: -3000px;
    background: #fafafa;
    position: absolute;
}
.ar-dv .ar-tit{
    margin-bottom: 0px;
    font-size: 34px;
}
.arenda-ts{

}
.arenda-ts p{
    font-size: 14px;
    margin-bottom: 0px;
    margin-top: 10px;
}
.arenda-ts a{
    display: block;
}
.arenda-ts a img{
    width: 100%;
}
.arenda-ts .inf{
    color: #777;
    margin-top: 15px;
}
.arenda-ts .img{
    position: relative;
}
.arenda-ts .inf .title{
    color: #222;
    font-size: 18px;
}
.arenda-ts .inf .addr{

}
.ar-stat{
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    padding-left: 15px;
    padding-right: 15px;
    padding-bottom: 10px;
    padding-top: 70px;
    color: white;
    display: flex;
    font-size: 13px;
    background: linear-gradient(to bottom, rgba(0,0,0,0) 0%,rgba(0,0,0,0.65) 96%,rgba(0,0,0,0.65) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00000000', endColorstr='#a6000000',GradientType=0 );
}
.ar-stat .itm{
    margin-right: 20px;
}
.ar-stat .itm:last-child{
    margin-right: 0px;
}
.ar-stat .itm i{
    margin-right: 4px;
}
.arenda-ts .ar-fv{
    position: absolute;
    bottom:10px;
    right: 15px;
    z-index: 10;
    font-size: 13px;
}
.arenda-ts .ar-fv:hover{
    opacity: 0.6;
}
.arenda-ts .price{
    background: #ffe65a;
    border-radius: 3px;
    color: #222;
    font-size: 14px;
    position: absolute;
    left: 15px;
    top:10px;
    z-index: 10;
    padding-left: 8px;
    padding-right: 8px;
    padding-bottom: 4px;
    padding-top: 4px;
}
.arenda-slider{
    overflow: initial!important;
}
.arenda-sect::after{
    content: "";
    top:0;
    bottom: 0;
    z-index: 10;
    right: 0;
    width: 200px;
    position: absolute;
    background: -moz-linear-gradient(left, rgba(255,255,255,0) 0%, rgba(250,250,250,1) 96%, rgba(250,250,250,1) 100%); /* FF3.6-15 */
    background: -webkit-linear-gradient(left, rgba(255,255,255,0) 0%,rgba(250,250,250,1) 96%,rgba(250,250,250,1) 100%); /* Chrome10-25,Safari5.1-6 */
    background: linear-gradient(to right, rgba(255,255,255,0) 0%,rgba(250,250,250,1) 96%,rgba(250,250,250,1) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00ffffff', endColorstr='#fafafa',GradientType=1 ); /* IE6-9 */
}
</style>