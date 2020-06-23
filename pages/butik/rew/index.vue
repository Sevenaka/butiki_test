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