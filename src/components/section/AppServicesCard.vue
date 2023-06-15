<script>

export default {
    name: 'AppServicesCard',
    props: {
        details: Object,
    }
}

</script>

<template>
    <div class="card">
        <img :src="details.image" alt="image">
        <h3>{{ details.service }}</h3>
        <span>{{ details.description }}</span>
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

    img {
        height: 100px;
    }

    h3 {
        color: $arancio;
        margin: 30px 0 30px 0;
    }

    span {
        color: $grigio;
    }
}
</style>