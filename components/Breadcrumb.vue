<template>
    <div class="brd">
        <ul>    
            <li><a href="#">Главная</a></li>
            <li><a href="#">Бутики</a></li>
            <li><a href="#">SUVARI</a></li>
        </ul>
    </div>
</template>

<style>
.brd{
    padding-bottom: 30px;
}
.brd ul{
    padding: 0px;
    margin: 0px;
    display: flex;
}
.brd ul li{
    list-style: none;
    position: relative;
}
.brd ul li::after{
    content: "/";
    display: block;
    float: right;
    margin-left: 16px;
    margin-right: 16px;
    color: #dedede;
}
.brd ul li:last-child::after{
    display: none;
}
.brd ul li a{
    color: #777;
}
.brd ul li a:hover,
.brd ul li:last-child a{
    color: #222;
}
</style>