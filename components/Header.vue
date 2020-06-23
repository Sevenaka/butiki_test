<template>
    <header>
      <div class="line-1 line">
        <div class="container">
          <div class="row">
            <div class="col-md-3 relative">
              <div class="nav-left">
                <div class="logo">
                  <nuxt-link to="/">
                    <img src="~/static/newlogo.png" />
                  </nuxt-link>
                </div>
                <div class="city">
                  <span @click="actionMenu()" class="city-btn">Каталог товаров <i class="fas fa-caret-down"></i></span>
                </div>
              </div>

              <div :class="['fix-menu', {'hide' : !menuOpen}]">
                <div class="menu-cnt">
                  <div class="menu-table">
                    <ul class="menu main-menu">
                      <li><a @mouseover="mouseoverSubmenu(1)" @mouseleave="subMenu = null" href="#">Женщинам <i class="fas fa-chevron-right"></i></a></li>
                      <li><a @mouseover="mouseoverSubmenu(2)" @mouseleave="subMenu = null" href="#">Межчинам <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Детям <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Товары для дома <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Досуг, спорт, туризм <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Красота, здоровье <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Мебель <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Украшения, аксессуары <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Зоотовары <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Антиквариат <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#" class="menu-im"><img src="~/static/balloons.svg">День всех влюбленных</a></li>
                      <li><a href="#" class="menu-im"><img src="~/static/stationery.svg">Снова в школу</a></li>
                    </ul>
                    <ul :class="['menu sub-menu', {'hide': subMenu != 1}]">
                      <li><a href="#">Одежда <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Обувь <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Будущие мамы <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Аксессуары <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Красота <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Спорт <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Разное <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Нижнее белье <i class="fas fa-chevron-right"></i></a></li>
                    </ul>
                    <ul :class="['menu sub-menu', {'hide': subMenu != 2}]">
                      <li><a href="#">Одежда <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Обувь <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Аксессуары <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Спорт <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Разное <i class="fas fa-chevron-right"></i></a></li>
                      <li><a href="#">Нижнее белье <i class="fas fa-chevron-right"></i></a></li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-md-5">
              <div class="search">
                <button class="src-btn"><i class="fas fa-search"></i></button>
                <input type="text" name="search" placeholder="Поиск товаров" />
              </div>
            </div>
            <div class="col-md-2">
              <a href="#" class="skd-lnk">
                <i class="fas fa-street-view"></i> Скидки рядом
              </a>
            </div>
            <div class="col-md-2">
              <nav class="us-nav">
                <ul>
                  <li><a href="#"><i class="fas fa-map-marker-alt"></i></a></li>
                  <li><a href="#"><span class="nt">8</span><i class="fas fa-shopping-cart"></i></a></li>
                  <li><a href="#"><span class="nt">3</span><i class="fas fa-heart"></i></a></li>
                  <li><a href="#"><i class="fas fa-sign-in-alt"></i></a></li>
                </ul>
              </nav>
            </div>
          </div>
        </div>
      </div>
    </header>
</template>

<script>
export default {
  data () {
    return {
        menuOpen: false,
        subMenu: null,
    }
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