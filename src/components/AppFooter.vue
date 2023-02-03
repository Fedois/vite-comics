<script>
export default {
    name: 'AppFooter',
    data() {
      return {
        linksBuy: [
            {
                img: 'buy-comics-digital-comics.png',
                name: 'carachters',
            },
            {
                img: 'buy-comics-merchandise.png',
                name: 'comics',            
            },
            {
                img: 'buy-comics-subscriptions.png',
                name: 'movies',
            },
            {
                img: 'buy-comics-shop-locator.png',
                name: 'tv',
                resize: 'special-img',
            },
            {
                img: 'buy-dc-power-visa.svg',
                name: 'games',
            },
        ],
        listComic: [
            {
                name: 'carachters',
            },
            {
                name: 'comics',            
            },
            {
                name: 'movies',
            },
            {
                name: 'TV',
            },
            {
                name: 'games',
            },
            {
                name: 'videos',
            },
            {
                name: 'news',
            },
        ],
        listShop: [
            {
                name: 'shop DC',
            },
            {
                name: 'shop DC Collectibles',
            },
        ],
        listDC: [
            {
                name: 'terms of use',
            },
            {
                name: 'privacy policy (new)',            
            },
            {
                name: 'ad choices',
            },
            {
                name: 'advertising',
            },
            {
                name: 'jobs',
            },
            {
                name: 'subscriptions',
            },
            {
                name: 'talent',
            },
            {
                name: 'workshops',
            },
            {
                name: 'CPSC',            
            },
            {
                name: 'certificates',
            },
            {
                name: 'ratings',
            },
            {
                name: 'shop help',
            },
            {
                name: 'contact us',
            },
        ],
        listSites: [
            {
                name: 'DC',
            },
            {
                name: 'MAD',            
            },
            {
                name: 'magazine',
            },
            {
                name: 'DC kids',
            },
            {
                name: 'DC',
            },
            {
                name: 'universe',
            },
            {
                name: 'DC power visa',
            },
        ],
        listSocial: [
            {
                img: 'footer-facebook.png',
            },
            {
                img: 'footer-twitter.png',
            },
            {
                img: 'footer-youtube.png',
            },
            {
                img: 'footer-pinterest.png',
            },
            {
                img: 'footer-periscope.png',
            },
        ]
        
      }
    },
    methods: {
        getImagePath: function(imgPath){
            return new URL (imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <footer>
        <section class="section-top">
            <div class="small-container">
                <ul class="list-buy">
                    <li v-for="link in linksBuy">
                        <a href="#">
                            <img :src="getImagePath(`../assets/img/${link.img}`)" alt="">
                            {{ link.name }}
                        </a>
                    </li>
                </ul>
            </div>
        </section>
        
        <section class="section-middle">
            <div class="container">

                <div class="list-container">
                    <div id="comics-and-shop">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="link in listComic">
                                <a href="#">{{ link.name }}</a>
                            </li>
                        </ul>

                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="link in listShop">
                                <a href="#">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                
                    <div id="dc">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="link in listDC">
                                <a href="#">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                
                    <div id="SITES">
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="link in listSites">
                                <a href="#">{{ link.name }}</a>
                            </li>
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
                        <li v-for="social in listSocial">
                            <a href="#">
                                <img :src="getImagePath(`../assets/img/${social.img}`)" alt="">
                            </a> 
                        </li>
                    </ul>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
/* section top */
.section-top{
    background-color: rgb(0, 128, 255);

    .small-container{
        max-width: 1100px;
        margin: 0 auto;
        height: 130px;

        > .list-buy{
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

                li > a{
                color: white;
                text-transform: uppercase;

                > img{
                    width: 50px;
                    vertical-align: middle;
                    margin-right: 10px;
                }
            }
        }
    }

}
// .special-img{
//     width: 40px;
// }

/* section-middle */
.section-middle{
    background: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    overflow: hidden;
}
.container{
    display: flex;

    .list-container{
        padding-top: 20px ;
        display: flex;
        color: white;
        width: 50%;

        > div{
            margin-right: 30px;

            h3{
                margin: 15px 0;
            }
            a{
                color: rgb(173, 168, 168);
                text-transform: capitalize;
            }
        }
    }
    .big-logo{
        width: 50%;
        position: relative;

        > img{
            position: absolute;
            top: -100px;
            left: 0;
        }
    }
}

/* inizio section bottom */
.section-bottom{
    height: 100px;
    background-color: rgb(27, 27, 27);

    .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button{
            padding: 10px;
            background-color: transparent;
            border: 1px solid rgb(0, 128, 255);

            > a{
                color: white;
            }
        }
        .follow { 
            > h3{
                color: rgb(0, 128, 255);
                display: inline-block;
                margin-right: 20px;
                vertical-align:middle;
            }

            .list-social{
                display: inline-block;

                > li{
                    display: inline-block;

                    img{
                        margin: 0 5px;
                        vertical-align: middle;
                        width: 30px;
                    }
                }
            }
        }
    }
}
</style>
