<script>

export default {
    name: 'AppHeaderHamburger',

}

</script>

<template>
    <div class="modal-dialog modal-fullscreen">
        <div class="close">
            <i class="fa-sharp fa-regular fa-xmark"></i>
        </div>

        <div class="list">
            <ul>
                <li>Home</li>
                <li>About Us</li>
                <li>Services</li>
                <li>Shop</li>
                <li>Our Team</li>
                <li>Blog</li>
                <li>Contact us</li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;




.modal-fullscreen {
    height: 100vh;
    width: 100vw;
    background-color: black;
    display: none;
    position: absolute;
    top: 0;
    left: 0;
    position: fixed;
    z-index: 999;
    font-style: none;


}
</style>