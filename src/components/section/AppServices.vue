<script>
import AppServicesCard from './AppServicesCard.vue'

export default {
    name: 'AppServices',
    components: {
        AppServicesCard
    },


    data() {
        return {
            cards: [
                {
                    imageName: '../../assets/images/avadabarbers-trimcut-icon-before.png',
                    "service": 'Trim & Cut',
                    "description": 'Avada Barbers are experts in the lickety split trim and hair cut. Quickbut careful and ridiculously good looking.'
                },
                {
                    imageName: 'avadabarbers-washndry-icon.png',
                    "service": 'Wash & Dry',
                    "description": 'Take a seat in our fine leather chairs lean back and let us lather you a fresh head in a luxurious fashion'
                },
                {
                    imageName: 'avadabarbers-beardtrim-icon.png',
                    "service": 'Beard Tidy',
                    "description": 'Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services form Avada Barbers'
                }
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }

}

</script>

<template>
    <section>
        <div class="services">
            <span>MENS GROOMING</span>
            <h1>Services</h1>

            <!-- riga servizi -->
            <div class="row">
                <AppServicesCard v-for="(card, index) in cards" :key="index" :details="card" />

            </div>

            <button>READ OBOUT OUR SERVICES</button>

            <div class="img">
                <img src="../../../public/triangle.svg" alt="">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

section {

    .services {
        @include my-display-flex-column($type: 'center');
        height: 100%;

        span {
            color: $arancio;
        }

        h1 {
            font-size: 60px;
            color: $grigio;
        }

        .row {
            @include my-display-flex-row;
        }

        .img {
            margin-top: 100px;
            width: 100%;
            filter: invert(1);

            img {
                width: 100%;
                height: 50%;
            }
        }
    }
}
</style>