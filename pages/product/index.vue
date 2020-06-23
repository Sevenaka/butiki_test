<template>
    <div class="product-page">
        <Header />
        <div class="rek-line">
            <div class="container">
                <div class="row">
                    <div class="col-md-12">
                        <div class="bn-flex">
                            <div class="itm">Сегодня -2 <img :src="require('~/static/thermometer.svg')" /></div>
                            <div class="itm">Завтра -22 </div>
                            <div class="itm itm-pd">БОЛЬШОЙ КАТАЛОГ ЗИМНИХ ТОВАРОВ!</div>
                            <div class="itm"><button class="white-btn">Купить</button></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="product-full">
            <div class="container">
                <div class="row">
                    <div class="col-md-5">
                        <div class="full-image">
                            <img :src="require('~/static/prod/full/fullprod.jpg')" />
                        </div>
                    </div>
                    <div class="col-md-4 text-infs">
                        <h1>Женская куртка</h1>
                    </div>
                    <div class="col-md-3">
                        3
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Header from '~/components/Header'
export default {
  data () {
    return {
       
    }
  },
  components: {
    Header
  },
  methods: {

  },
  mounted () {
    

  }
}
</script>

<style>
.rek-line{
    margin-bottom: 30px;
    padding-bottom: 8px;
    padding-top: 8px;
    background: url('~static/rekbg.jpg');
    background-position: center;
    color: white;
}
.product-full{
    
}
.full-image{

}
.full-image img{
    width: 100%;
    max-height: 600px;
}
.bn-flex{
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
    text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.20);
}
.bn-flex img{
    width: 28px;
    margin-left: 20px;
}
.bn-flex .itm{
    margin-right: 20px;
}
.itm-pd{
    padding-left: 40px;
}
.white-btn{
    border: 1px solid white;
    border-radius: 3px;
    color: white;
    font-weight: bold;
    cursor: pointer;
    background: transparent;
    text-transform: uppercase;
    font-size: 13px;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 3px;
    padding-top: 3px;
    display: inline-block;
    margin-left: 30px;
}
.white-btn:hover{
    background: rgba(255, 255, 255, 0.3);
}
</style>