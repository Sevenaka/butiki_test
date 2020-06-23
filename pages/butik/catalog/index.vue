<template>
    <div class="butik-page">
        <Header />
        <div class="butik-full">
            <div class="container">
                <div class="row">
                    <div class="col-md-12">
                        <Breadcrumb />
                    </div>
                    <div class="col-md-3">
                        <div class="butik-main-inf">
                            <div class="b-sect">
                                <div class="b-logo">
                                    <img :src="require('~/static/logo/logo2.jpg')" />
                                    <h1 class="b-title">SUVARI</h1>
                                    <p class="b-desc">Магазин женской одежды</p>
                                    <ul class="b-soc">
                                        <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                                        <li><a href="#"><i class="fab fa-vk"></i></a></li>
                                        <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="cat-filter">
                            <div class="fltr-field">
                                <div class="lab">Диапазон цен тг.</div>
                                <div class="row price-row">
                                    <div class="col-md-6">
                                        <input class="" type="text" placeholder="От" />
                                    </div>
                                    <div class="col-md-6">
                                        <input type="text" placeholder="До" />
                                    </div>
                                </div>
                            </div>
                            <div class="fltr-field">
                                <div class="lab">Материал</div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Кожа</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Шелк</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Хлопок</label>
                                </div>
                                <div class="al-chc">
                                    <span>Показать еще</span>
                                </div>
                            </div>
                            <div class="fltr-field">
                                <div class="lab">Страна производтитель</div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Россия</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Китай</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Турция</label>
                                </div>
                                <div class="al-chc">
                                    <span>Показать еще</span>
                                </div>
                            </div>
                            <div class="fltr-field">
                                <div class="lab">Размер</div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>45-47</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>50-52</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>60-72</label>
                                </div>
                                <div class="al-chc">
                                    <span>Показать еще</span>
                                </div>
                            </div>
                            <div class="fltr-field">
                                <div class="lab">Модель</div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Футболка</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Майка</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Поло</label>
                                </div>
                                <div class="al-chc">
                                    <span>Показать еще</span>
                                </div>
                            </div>
                            <div class="fltr-field">
                                <div class="lab">Цвет</div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Белый</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Красный</label>
                                </div>
                                <div class="field-chc">
                                    <input type="checkbox">
                                    <label>Черный</label>
                                </div>
                                <div class="al-chc">
                                    <span>Показать еще</span>
                                </div>
                            </div>
                        </div>
                        <div class="pop-lnk">
                            <label>Смотрите также</label>
                            <a href="#">Мужская одежда</a>, 
                            <a href="#">Женская одежда</a>, 
                            <a href="#">Женские очки</a>, 
                            <a href="#">Трусики</a>, 
                            <a href="#">Кофты</a>, 
                            <a href="#">Женская куртка</a>,
                            <a href="#">Кеды</a>,
                            <a href="#">Кожанка</a>
                        </div>
                    </div>
                    <div class="col-md-9">
                        <div class="b-main-info">
                            <butik-menu />
                            <div class="about-text">
                                <div class="row">
                                    <div class="col-md-12">
                                        <div class="sort">
                                            <div class="tit">
                                                Сортировать: 
                                            </div>
                                            <div class="itm">
                                                <span class="active">Новые</span>
                                            </div>
                                            <div class="itm">
                                                <span>Дешевые</span>
                                            </div>
                                            <div class="itm">
                                                <span>Дорогие</span>
                                            </div>
                                            <div class="itm">
                                                <span>Скидка</span>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская зимняя куртка" price="8 200" image="prod7.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Китайская курта" price="600" image="prod8.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Кеды Nike" price="4 500" image="prod2.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Пуховик" price="2 600" image="prod3.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская зимняя куртка" price="8 200" image="prod7.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Китайская курта" price="600" image="prod8.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="13 000" image="prod6.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская зимняя куртка" price="8 200" image="prod7.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Китайская курта" price="600" image="prod8.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Абибас" price="1 300" image="prod9.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod color="black" title="Черные кеды" price="9 000" image="prod10.jpg" />
                                    </div>
                                    <div class="prod-col col-md-3">
                                        <Prod title="Женская куртка" price="1 000" image="prod1.jpg" />
                                    </div>
                                    <div class="col-md-12">
                                        <ul class="pager-b">
                                            <li class="prev"><a href="#"><i class="fas fa-chevron-left"></i> Назад</a></li>
                                            <li><a href="#">1</a></li>
                                            <li><a href="#">2</a></li>
                                            <li class="active"><a href="#">3</a></li>
                                            <li><a href="#">4</a></li>
                                            <li><a href="#">5</a></li>
                                            <li><a href="#">6</a></li>
                                            <li class="next"><a href="#">Вперед <i class="fas fa-chevron-right"></i></a></li>
                                        </ul>
                                    </div>
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
import Footer from '~/components/Footer'
import ButikInfo from '~/components/Butikinfo'
import ButikMenu from '~/components/ButikMenu'
import Prod from '~/components/Prod'
export default {
  data () {
    return {

    }
  },
  components: {
    Header,
    Breadcrumb,
    Prod: Prod,
    Footer,
    ButikInfo: ButikInfo,
    ButikMenu: ButikMenu
  },
  methods: {

  },
  mounted () {
    

  }
}
</script>

<style>
.about-text{
    padding-bottom: 40px;
}
.sort{
    margin-bottom: 40px;
    display: flex;
    align-items: center;
}
.sort .tit{
    font-weight: bold;
    margin-right: 10px;
}
.sort .itm{
    margin-left: 10px;
}
.sort .itm span{
    cursor: pointer;
    display: block;
    color: #222;
    border-radius: 3px;
    padding-bottom: 6px;
    padding-top: 6px;
    padding-left: 12px;
    padding-right: 12px;
}
.sort .itm span.active{
    background: #ffe65a;
}
.cat-filter{
    margin-top: 30px;
    padding: 30px;
    background: rgba(0, 0, 0, 0.06);
    border-radius: 5px;
}
.cat-filter .fltr-field{
    padding-bottom: 20px;
    padding-top: 20px;
    border-bottom: 1px solid rgba(204, 204, 204, 0.7);
}
.cat-filter .fltr-field .lab{
    font-weight: bold;
    display: block;
    margin-bottom: 8px;
}
.cat-filter .fltr-field:first-child{
    padding-top: 0px;
}
.cat-filter .fltr-field:last-child{
    padding-bottom: 0px;
    border-bottom: 0px;
}
.cat-filter .fltr-field .field-chc{
    position: relative;
    padding-left: 22px;
}
.cat-filter .fltr-field .field-chc input{
    display: none;
}
.cat-filter .fltr-field .field-chc label{
    cursor: pointer;
}
.cat-filter .fltr-field .field-chc label:hover{
    opacity: 0.6;
}
.cat-filter .fltr-field .field-chc label::after{
    content: "";
    position: absolute;
    left: 0;
    top: 2px;
    width: 16px;
    height: 16px;
    border: 1px solid #222;
}
.cat-filter .al-chc{
    font-size: 14px;
    border-bottom: 1px dashed;
    color: #777;
    display: inline-block;
    cursor: pointer;
}
.price-row{
    margin-left: -5px!important;
    margin-right: -5px!important;
}
.price-row .col-md-6{
    padding-left: 5px!important;
    padding-right: 5px!important;
}
.price-row .col-md-6 input{
    width: 100%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 4px;
    padding-top: 4px;
    font-size: 14px;
    border-radius: 3px;
    border: 1px solid #cecece;
}
.pop-lnk{
    padding: 30px;
}
.pop-lnk label{
    display: block;
    font-weight: bold;
    margin-bottom: 5px;
}
</style>