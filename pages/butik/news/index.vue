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
                            <div class="about-text">
                                <div class="row">
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
export default {
  data () {
    return {

    }
  },
  components: {
    Header,
    Breadcrumb,
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
</style>