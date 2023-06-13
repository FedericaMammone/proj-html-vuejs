<script>
export default {
    name: 'AppProducts',

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
                <div class="card"></div>
                <div class="card"></div>
                <div class="card"></div>
                <div class="card"></div>
            </div>

            <button></button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;
</style>