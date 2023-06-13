<script>
import AppProductsCard from './AppProductsCard.vue'
import AppProductsButter from './AppProductsButter.vue'

export default {
    name: 'AppProducts',
    components: {
        AppProductsCard,
        AppProductsButter
    },

    data() {
        return {
            cards: [
                {
                    "image": '../../../public/brush_dark-400x400.png',
                    "name": 'Brush',
                    "price": '$15.00'
                },
                {
                    "image": '../../../public/scissors-400x400.png',
                    "name": 'Scissors',
                    "price": '$85.00'
                },
                {
                    "image": '../../../public/hot_oil_dark-400x400.png',
                    "name": 'Hot Oil',
                    "price": '$15.00'
                },
                {
                    "image": '../../../public/straight_razor_dark-400x400.png',
                    "name": 'Straight Razor',
                    "price": '$30.00'
                }
            ]
        }
    },

}

</script>

<template>
    <section>
        <!-- container sezione prodotti -->
        <div class="products">
            <span>WE HAVE YOU COVERED</span>
            <h1>Avada Grooming Products</h1>

            <!-- riga  prodotti-->
            <div class="row">
                <AppProductsCard v-for="card in cards" :details="card" />
            </div>

            <button>SHOP OUR PRODUCT RANGE</button>

            <AppProductsButter />
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

section {
    background-image: url(../../assets/images/avadabarbers-reviewsbackground.jpg);
    min-height: 800px;
    background-size: cover;
    background-repeat: no-repeat;

    .products {
        @include my-display-flex-column($type: 'center');
        height: 100%;
        position: relative;

        span {
            color: $arancio;
        }

        h1 {
            font-size: 60px;
            color: $grigio;
        }

        .row {
            @include my-display-flex-row;
            gap: 30px;
        }
    }
}
</style>