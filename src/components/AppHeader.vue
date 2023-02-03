<script>
export default {
    name: 'AppHeader',
    data() {
      return {
        linksNav: [
            {
                name: 'carachters',
                active: false,
            },
            {
                name: 'comics',
                active: true,
            },
            {
                name: 'movies',
                active: false,
            },
            {
                name: 'tv',
                active: false,
            },
            {
                name: 'games',
                active: false,
            },
            {
                name: 'collectibles',
                active: false,
            },
            {
                name: 'videos',
                active: false,
            },
            {
                name: 'fans',
                active: false,
            },
            {
                name: 'news',
                active: false,
            },
            {
                name: 'shop',
                active: false,
            },
        ]
        
      }
    }
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
                    <li v-for="link in linksNav">
                        <a :class="{'active': link.active == true}" href="#">{{ link.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header{
    position: sticky;
    top: 0;
    background-color: white;
    z-index: 30;

    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;

        .logo > img{
            width: 80px;
        }

        nav{
            height: 100%;

            > ul{
                font-size: 0.85em;

                > li{
                    display: inline-block;
                    line-height: 100px;
                    height: 100%;

                    > a{
                        margin: 0 10px;
                        text-decoration: none;
                        color: rgb(54, 54, 54);
                        text-transform: uppercase;
                        font-weight: bold;

                        &.active{
                            color: rgb(0, 128, 255);
                        }
                    }
                }
            }
        }
    }

}
</style>
