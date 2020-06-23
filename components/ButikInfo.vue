<template>
    <div class="col-md-4">
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
            <div class="b-sect">
                <div class="b-field">
                    <label>Адрес:</label>
                    <p>г.Усть-Каменогорск, пр. Независимости, 26.</p>
                    <p><i class="fas fa-map-marker-alt"></i> <span class="aj-lnk">Показать на карте</span></p>
                </div>
                <div class="b-field">
                    <label>Торговый центр:</label>
                    <p><a href="#">ЦУМ</a> - 1 этаж, №202</p>
                </div>
                <div class="b-field">
                    <label>Время работы:</label>
                    <p>10:00 - 20:00 (Пн - Вс)</p>
                </div>
                <div class="b-field">
                    <label>Телефоны:</label>
                    <p>+7 (705) <span class="aj-lnk">Показать телефоны</span></p>
                </div>
                <div class="b-field">
                    <label>Особенности:</label>
                    <p>Кабинка для переодевания, Парковка</p>
                </div>
                <div class="b-field">
                    <label>Принимаемые к оплате карты: </label>
                    <p>Visa, Visa Electron, MasterCard/Eurocard, Maestro, American Express, China UnionPay, Altyn, Union Card</p>
                </div>
            </div>
            <div class="b-sect">
                <div class="b-r-title">Как вам бутик?</div>
                <div class="b-r-btn-grp">
                    <div class="itm"><button class="b-r-btn"><i class="fas fa-thumbs-up"></i> Понравился</button></div>
                    <div class="itm"><button class="b-r-btn"><i class="fas fa-thumbs-down"></i></button></div>
                </div>
                <div class="b-rate">
                    <div class="rate-i">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                    </div>
                    <span class="cnt">У этого магазина <a href="#">4 отзыва</a></span>
                </div>
            </div>
        </div>
        <div class="view pd30">
            8902 человека интересовались этим бутиком
        </div>
        <div class="but-soc-rp">
            <label>Поделиться этим бутиком</label>
            <ul>
                <li><a href="#"><i class="fab fa-vk"></i></a></li>
                <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fab fa-odnoklassniki"></i></a></li>
                <li><a href="#"><i class="fab fa-whatsapp"></i></a></li>
                <li><a href="#"><i class="fab fa-telegram-plane"></i></a></li>
                <li><a href="#"><i class="fab fa-twitter"></i></a></li>
            </ul>
        </div>
    </div>
</template>