<script>

export default {
    name: 'AppProductsButter',

}

</script>

<template>
    <div class="butter">
        <div class="left">
            <img src="../../assets/images/shaving_butter-400x400.png" alt="">
        </div>
        <div class="right">
            <span>THIS MONTHS FEATURED PRODUCT</span>
            <h2>Shaving Butter</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae dolor voluptates tenetur quod, facilis odio
                modi temporibus consequuntur quas quisquam provident rem, necessitatibus eaque nulla cum minima suscipit
                earum. Ea.</p>

            <button>BUY NOW</button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
;
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

.butter {
    border-top: 3px solid $arancio;
    height: 303px;
    width: 900px;
    background-color: #121413;
    position: absolute;
    bottom: -450px;

    .left {
        width: 300px;
        height: 300px;
        background-image: url(../../assets/images/avadabarbers-cta-background.jpg);
        background-size: cover;
        position: relative;
        float: left;

        img {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 250px;

        }
    }

    .right {
        @include my-display-flex-column;
        width: 600px;
        height: 300px;
        padding: 0 40px;
    }

    span {
        color: $arancio;
    }

    h2 {
        color: $grigio;
        font-size: 50px;
        margin-bottom: 20px;
    }

    p {
        color: rgba($color: $grigio, $alpha: 0.5);
        font-size: 14px;
        line-height: 25px;
    }

}
</style>