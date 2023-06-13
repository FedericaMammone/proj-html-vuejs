<script>
export default {
    name: 'AppBarbers',

}

</script>

<template>
    <section>
        <div class="barbers">
            <div class="text">
                <span>AWARD WINNING</span>
                <h1>Pro Barbers</h1>
                <button>MEET YOUR NEW BARBER</button>
            </div>


            <div class="img">
                <img src="../../../public/triangle.svg" alt="">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

section {
    height: 500px;
    background-image: url(../../assets/images/avadabarbers-about-introbackground.jpg);
    background-size: 100%;


    .barbers {
        @include my-display-flex-column($type: 'center');
        height: 100%;
        position: relative;

        .text {
            text-align: center;
            margin-bottom: 80px;

            span {
                color: $arancio;
            }

            h1 {
                font-size: 60px;
                color: $grigio;
                margin: 10px 0 20px 0;
            }
        }



        .img {
            position: absolute;
            bottom: 0;
            width: 100%;

            img {
                width: 100%;
                height: 50%;
            }
        }
    }
}
</style>