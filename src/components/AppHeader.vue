<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li><a href="#">charachters</a></li>
                    <li><a href="#" class="active">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">collectibles</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">fans</a></li>
                    <li><a href="#">news</a></li>
                    <li><a href="#">shop</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header{
    position: sticky;
    top: 0;
    background-color: white;
    z-index: 30
}
.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}
.logo > img{
    width: 80px;
}
nav{
    height: 100%;
}
nav > ul{
    font-size: 0.85em;
}
ul > li{
    display: inline-block;
    line-height: 100px;
    height: 100%;
}

ul li a{
    margin: 0 10px;
    text-decoration: none;
    color: black;
    text-transform: uppercase;
}
a.active{
    color: blue;
}
</style>
