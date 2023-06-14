<script>
export default {
    name: 'AppFooter',

}

</script>

<template>
    <footer>
        <!-- footer -->
        <div class="row">

            <div class="card">
                <img src="../assets/images/avadabarbers_footer_shop_image-300x234.png" alt="">
                <button>SHOP OUR RANGE NOW</button>
            </div>

            <div class="info">
                <img src="../assets/images/avadabarbers-logo-x2-200x70.png" alt="logo-footer">
                <ul>
                    <li><a href="#">Avada Barbers</a></li>
                    <li><a href="#">123 New York Street</a></li>
                    <li><a href="#">New York City</a></li>
                    <li><a href="#">info@yourwebsite.com</a></li>
                    <li><a href="#">+1 (555) 555-1212</a></li>
                </ul>

                <span><strong>FOLLOW US</strong></span>

                <div class="social">
                    <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="#"><i class="fa-brands fa-twitter"></i></a>
                    <a href="#"><i class="fa-brands fa-youtube"></i></a>
                    <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </div>
            </div>

            <div class="card">
                <img src="../assets/images/avadabarbers_footer_appointment_image-300x234.png" alt="">
                <button>BOOK YOUR APPOINTMENT</button>
            </div>
        </div>

        <!-- copyright -->
        <div class="copyright">
            <span> &copy; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights | Powered by WordPress</span>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

footer {
    min-height: 500px;
    background-color: #121314;

    .row {
        @include my-display-flex-row('center');
        --bs-gutter-x: 0;

        .card,
        .info {
            @include my-display-flex-column('center');
            margin: 50px 20px;
            width: 300px;

            border: none;
            text-align: center;
            background-color: #121314;

            img {
                margin-bottom: 40px;
            }

            ul {
                padding-left: 0;
                margin-bottom: 40px;

                li,
                a {
                    color: rgba($color: $grigio, $alpha: 0.5);
                }
            }

            span {
                color: $arancio;
                margin-bottom: 30px
            }

            .fa-brands {
                color: $grigio;
            }
        }
    }

    .copyright {
        @include center($type: 'both');
        height: 100px;
        background-color: #161718;

        span {
            color: rgba($color: $grigio, $alpha: 0.2);
        }
    }

}
</style>