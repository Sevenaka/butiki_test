<template>
    <div class="prod prod-teas">
        <div class="lk">
            <span :class="[{'white' : color}]"><i class="far fa-heart"></i></span>
        </div>
        <a href="#">
            <div class="prod-img">
                <img :src="require('~/static/prod/' + image)" />
            </div>
            <div class="inf">
                <div class="title">{{title}}</div>
                <div class="price">{{price}} тг.</div>
            </div>
        </a>
    </div>
</template>

<script>
export default {
  props: {
      title: String,
      image: String,
      price: String,
      color: String
  }
}
</script>

<style>
.prod-teas{
    position: relative;
    background: white;
}
.prod-teas > a{
    display: block;
    color: #777;
}
.prod-teas img{
    width: 100%;
    max-height: 275px;
}
.prod-teas .inf{
    margin-top: 15px;
}
.prod-teas .inf .title{
    color: #222;
}
.prod-teas .inf .price{
    color: #777;
}
.prod-img{
    text-align: center;
}
.prod-teas:hover .inf .title{
    color: #ff280c;
}
.prod-teas .lk{
    position: absolute;
    z-index: 10;
    right: 10px;
    top: 10px;
}
.prod-teas .lk span{
    cursor: pointer;
    display: block;
}
.prod-teas .lk span.white{
    color: white;
}
.prod-teas .lk span:hover{
    color:#f55b62;
}
.prod-teas:hover{
    box-shadow: 0 0px 3px rgba(4,4,4,0.2);
}
</style>