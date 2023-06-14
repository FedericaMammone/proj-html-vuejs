<script>
export default {
    name: 'AppReviews',

}

</script>

<template>
    <div class="reviews">
        <span>WHAT PEOPLE SAY</span>
        <h1>Reviews</h1>

        <div class="row">
            <div class="card">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Optio aliquid animi a sed temporibus laudantium
                    hic magnam similique corporis excepturi, dolorum architecto saepe, exercitationem ab nisi libero
                    doloribus eius perferendis?</p>
                <div class="image">
                    <img src="../../assets/images/avadabarbers-trimcut-gallery6-200x200.jpg" alt="">
                </div>

                <span><i>Jhon Doe</i></span>
            </div>
            <div class="card">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Optio aliquid animi a sed temporibus laudantium
                    hic magnam similique corporis excepturi, dolorum architecto saepe, exercitationem ab nisi libero
                    doloribus eius perferendis?</p>
                <div class="image">
                    <img src="../../assets/images/avadabarbers-trimcut-gallery7-200x201.jpg" alt="">
                </div>
                <span><i>Pete Jones</i></span>
            </div>
            <div class="card">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Optio aliquid animi a sed temporibus laudantium
                    hic magnam similique corporis excepturi, dolorum architecto saepe, exercitationem ab nisi libero
                    doloribus eius perferendis?</p>
                <div class="image">
                    <img src="../../assets/images/avadabarbers-trimcut-gallery3-200x201.jpg" alt="">
                </div>
                <span><i>Mark Wilson</i></span>
            </div>
        </div>

        <div class="triangle">
            <img src="../../../public/triangle.svg" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

.reviews {
    @include my-display-flex-column($type: 'center');
    height: 100%;
    position: relative;
    margin-top: 400px;

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

        .card {
            @include my-display-flex-column('center');
            margin: 50px 20px;
            width: 250px;
            border: none;
            text-align: center;

            img {
                height: 100px;
                border-radius: 50%;
            }
        }
    }

    .triangle {

        margin-top: 50px;
        width: 100%;
        transform: rotate(180deg);

        img {
            width: 100%;
            height: 50%;
        }

    }
}
</style>