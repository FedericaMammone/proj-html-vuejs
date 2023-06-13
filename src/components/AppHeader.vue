<script>
export default {
    name: 'AppHeader',

}

</script>

<template>
    <div class="container">
        <div class="distanziatore">
            <!-- barra naviigazione con logo e menù -->
            <nav>
                <!-- logo -->
                <div class="logo">
                    <img src="../assets/images/avadabarbers-logo-x1.png" alt="logo">
                </div>

                <!-- carrello e hamburger menù -->
                <div class="menu">
                    <i class="fa-solid fa-cart-shopping"></i>
                    <i class="fa-solid fa-bars"></i>
                </div>
            </nav>

            <div class="jumbo">
                <!-- sezione simil-jumbo -->
                <div class="barber-shop">
                    <h1>Barber Shop</h1>
                    <div class="linea"></div>
                    <span>The Pinnacle of Male Grooming</span>
                    <button>LEARN MORE</button>
                </div>

                <div class="image-right">
                    <img src="../assets/images/avadabarbers_hero_focalmirror-400x550.png" alt="">
                </div>
            </div>

        </div>


    </div>
</template>

<style lang="scss" scoped>
@use './../styles/general.scss' as *;
@use './../styles/partials/variables.scss' as *;
@use './../styles/partials/mixins.scss' as *;

.container {
    background-image: url(../assets/images/avadabarbers-homepage-hero-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 800px;
    max-width: 100%;
}

.distanziatore {
    width: 70%;
    margin: 0 auto;
    min-height: 200px;

    nav {
        width: 100%;

        @include my-display-flex-row;

        img {
            margin-top: 20px;
        }

        .menu {

            margin-top: 20px;

            .fa-solid {
                font-size: 20px;
                color: $primary;
                padding: 10px;

                &:hover {
                    cursor: pointer;
                }
            }
        }
    }

    .jumbo {
        @include my-display-flex-row;
    }

    .barber-shop {
        min-height: 100vh;
        color: $similBianco;
        @include my-display-flex-column;

        h1 {


            font-size: 60px;
        }

        .linea {
            width: 150px;
            border: 2px solid orange;
            margin: 20px 0 20px 0;
        }

        span {
            margin-bottom: 20px;
            color: rgba($color: grey, $alpha: 0.5);
        }


    }
}
</style>