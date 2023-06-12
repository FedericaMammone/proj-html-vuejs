<script>
export default {
    name: 'AppHeader',

}

</script>

<template>
    <div class="container">

        <!-- barra naviigazione con logo e menù -->
        <nav>
            <!-- logo -->
            <div class="logo">

            </div>

            <!-- carrello e hamburger menù -->
            <div class="menu">

            </div>
        </nav>

        <!-- sezione simil-jumbo -->
        <div class="barber-shop">

        </div>

        <div class="image-right">

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
</style>