<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <section class="section-top">
            <div class="small-container">
                <ul class="list-buy">
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            digital comic
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            dc merchandis
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            subscriptio
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img id="special-img" src="../assets/img/buy-comics-shop-locator.png" alt="">
                            comic shop locato
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            dc power vis
                        </a>
                    </li>
                </ul>
            </div>
        </section>
        
        <section class="jumbotron">
            <div class="container">

                <div class="list-container">
                    <div id="comics-and-shop">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li> <a href="#">characters</a> </li>
                            <li> <a href="#">comics</a> </li>
                            <li> <a href="#">movie</a> </li>
                            <li> <a href="#"> TV</a></li>
                            <li> <a href="#">games</a> </li>
                            <li> <a href="#">videos</a> </li>
                            <li> <a href="#">news</a> </li>
                        </ul>

                        <h3>SHOP</h3>
                        <ul>
                            <li><a href="#">shop DC</a></li>
                            <li><a href="#">shop DC Collectibles</a></li>
                        </ul>
                    </div>
                
                    <div id="dc">
                        <h3>DC</h3>
                        <ul>
                            <li><a href="#">Terms of use</a></li>
                            <li><a href="#">privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advetising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC certificates</a></li>
                            <li><a href="#">ratings</a></li>
                            <li><a href="#">shop help</a></li>
                            <li><a href="#">contact us</a></li>
                        </ul>
                    </div>
                
                    <div id="SITES">
                        <h3>SITES</h3>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC kids</a></li>
                            <li><a href="#">DC universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>

                <div class="big-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>
        
        <section class="section-bottom">
            <div class="container">
                <div class="sign">
                    <button><a href="#">SIGN-UP NOW!</a></button>
                </div>

                <div class="follow">
                    <h3>FOLLOW US</h3>
                    <ul class="list-social">
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="">
                            </a> 
                        </li>
                        <li>
                            <a href="#"> 
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </a> 
                        </li>
                        <li>
                            <a href="#"> 
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </a> 
                        </li>
                    </ul>
                </div>
            </div>
            
        </section>
    </footer>
</template>

<style scoped>
/* contenuto top */
.section-top{
    background-color: rgb(0, 128, 255);
}
.small-container{
    max-width: 1100px;
     margin: 0 auto;
    height: 130px;
}
            
.small-container > .list-buy{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.list-buy img{
    width: 50px;
    vertical-align: middle;
    margin-right: 10px;
}
#special-img{
    width: 40px;
}

.list-buy li > a{
    color: white;
    text-transform: uppercase;
}

/* inizio jumbotron */
.jumbotron{
    background: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    overflow: hidden;
}
.container{
    display: flex;

}
.list-container{
    padding-top: 20px ;
    display: flex;
    color: white;
    width: 50%;
}

.list-container > div{
    margin-right: 30px;
}

h3{
    margin: 15px 0;
}
ul li > a{
    color: rgb(173, 168, 168);
    text-transform: capitalize;
}
.big-logo{
    width: 50%;
    position: relative;
}

.big-logo img{
    position: absolute;
    top: -100px;
    left: 0;
}
.section-bottom{
    height: 100px;
    background-color: rgb(27, 27, 27);
}
.section-bottom > .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.sign > button{
    padding: 10px;
    background-color: transparent;
    border: 1px solid rgb(0, 128, 255);
}
.sign > button a{
    color: white;
}
.follow > h3{
    color: rgb(0, 128, 255);
    display: inline-block;
    margin-right: 20px;
    vertical-align:middle;
}
.list-social{
    display: inline-block;
}
.list-social > li{
    display: inline-block;
}
.list-social > li img{
    margin: 0 5px;
    vertical-align: middle;
    width: 30px;
}
</style>
