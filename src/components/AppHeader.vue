<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
    <header>
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#">
                        charachters
                    </a>
                </li>
                <li>
                    <a href="#" class="active">
                        comics
                    </a>
                </li>
                <li>
                    <a href="#">
                        movies
                    </a>
                </li>
                <li>
                    <a href="#">
                        tv
                    </a>
                </li>
                <li>
                    <a href="#">
                        games
                    </a>
                </li>
                <li>
                    <a href="#">
                        collectibles
                    </a>
                </li>
                <li>
                    <a href="#">
                        videos
                    </a>
                </li>
                <li>
                    <a href="#">
                        fans
                    </a>
                </li>
                <li>
                    <a href="#">
                        news
                    </a>
                </li>
                <li>
                    <a href="#">
                        shop
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 0;

    .logo{
        
        img{
            width: 80px;
        }
    }

    nav{
        ul{
        list-style: none;
        text-transform: uppercase;
        font-size: 0.75em;

        li{
            display: inline-block;
            padding: 20px 10px;

            a{
                text-decoration: none;
                color: black;

                &.active{
                    color: blue;
                }
            }
        }
    }
    }
}
</style>
