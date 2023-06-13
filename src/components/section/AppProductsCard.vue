<script>

export default {
    name: 'AppProductsCard',
    props: {
        details: Object,

    }
}

</script>

<template>
    <div class="card">
        <img :src="details.image" alt="image">
        <h3>{{ details.name }}</h3>
        <span>{{ details.price }}</span>
    </div>
</template>

<style lang="scss" scoped>
;
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

.card {
    @include my-display-flex-column('center');
    margin: 50px 20px;
    width: 250px;
    border: none;
    text-align: center;
    background-color: rgba($color: #000000, $alpha: 0);

    img {
        height: 300px;
        background-color: rgba($color: #000000, $alpha: 0);
    }

    h3 {
        color: $arancio;
    }

    span {
        color: $arancio;
    }
}
</style>