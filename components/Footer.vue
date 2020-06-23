<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-md-8">
                    <div class="menu-row">
                        <div class="fot-menu">
                            <label>Покупателям</label>
                            <ul>
                                <li><a href="#">Каталог товаров</a></li>
                                <li><a href="#">Новости магазинов</a></li>
                                <li><a href="#">Отзывы покупателей</a></li>
                                <li><a href="#">Модный блог</a></li>
                                <li><a href="#">Рекомендации покупателям</a></li>
                            </ul>
                        </div>
                        <div class="fot-menu">
                            <label>Продавцам</label>
                            <ul>
                                <li><a href="#">Как продавать на Butiki.kz</a></li>
                                <li><a href="#">Тарифы</a></li>
                                <li><a href="#">Аренда бутиков</a></li>
                                <li><a href="#">Продажа бутиков</a></li>
                                <li><a href="#">Пользовательское соглашение</a></li>
                                <li><a href="#">Политика конфиденциальности</a></li>
                            </ul>
                        </div>
                        <div class="fot-menu">
                            <label>О нас</label>
                            <ul>
                                <li><a href="#">О Butiki.kz</a></li>
                                <li><a href="#">Реклама на сайте</a></li>
                                <li><a href="#">Наши контакты</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 text-right">
                    <div class="anc"><i class="far fa-copyright"></i> 2019 Butiki.kz</div>
                    <div class="fot-soc">
                        <label>Следите за нами</label>
                        <ul>    
                            <li><a class="fb" href="#"><i class="fab fa-facebook-f"></i></a></li>
                            <li><a class="vk" href="#"><i class="fab fa-vk"></i></a></li>
                            <li><a class="inst" href="#"><i class="fab fa-instagram"></i></a></li>
                            <li><a class="od" href="#"><i class="fab fa-odnoklassniki"></i></a></li>
                        </ul>
                    </div>
                    <div class="mob-lnk">
                        <div class="itm"><img src="~/static/footer__icon-appstore.svg"></div>
                        <div class="itm"><img src="~/static/footer__icon-googleplay.svg"></div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style>
footer{
    background: #f3f3f3;
    padding-bottom: 50px;
    padding-top: 50px;
    border-top: 1px solid #dedede;
}
.fot-menu{
    font-size: 14px;
    margin-right: 100px;
}
.fot-menu:last-child{
    margin-right: 0px;
}
.fot-menu label{
    display: block;
    margin-bottom: 8px;
    color: #222;
    font-weight: bold;
}
.fot-menu ul{
    padding: 0px;
    margin: 0px;
}
.fot-menu ul li{
    list-style: none;
    margin-bottom: 8px;
}
.fot-menu ul li:last-child{
    margin-bottom: 0px;
}
.fot-menu ul li a{
    color: #777;
}
.fot-menu ul li a:hover{
    color: #222;
}
.text-right{
    text-align: right;
    color: #777;
}
.menu-row{
    display: flex;
}
.fot-soc{
    margin-top: 15px;
}
.fot-soc label{
    margin-bottom: 8px;
    display: block;
    font-size: 13px;
}
.fot-soc ul{
    display: flex;
    padding: 0px;
    margin: 0px;
    justify-content: flex-end;
}
.fot-soc ul li{
    list-style: none;
    margin-right: 10px;
}
.fot-soc ul li:last-child{
    margin-right: 0px;
}
.fot-soc ul li a{
    display: block;
    color: white;
    background: black;
    border-radius: 50%;
    width: 30px;
    height: 30px;
    text-align: center;
    line-height: 32px;
}
.fot-soc ul li a:hover{
    opacity: 0.6;
}
.fot-soc ul li a.vk{
    background: #5281b7;
}
.fot-soc ul li a.fb{
    background: #5281b7;
}
.fot-soc ul li a.od{
    background: #f7931e;
}
.mob-lnk{
    display: flex;
    margin-top: 40px;
    justify-content: flex-end;
}
.mob-lnk .itm{
    margin-left: 6px;
}
</style>