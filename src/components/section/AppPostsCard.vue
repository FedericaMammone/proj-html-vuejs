<script>

export default {
    name: 'AppPostsCard',
    props: {
        details: Object,

    }
}

</script>

<template>
    <div class="card">
        <img :src="details.image" alt="image">
        <h3>{{ details.title }}</h3>
        <p>{{ details.description }}</p>
    </div>
</template>

<style lang="scss" scoped>
;
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

.card {
    @include my-display-flex-column('center');
    justify-content: flex-start;
    margin: 50px 20px;
    width: 320px;
    border: none;
    text-align: center;
    background-color: $similBianco;


    img {
        height: 200px;
        margin-bottom: 20px;
    }

    h3 {
        color: $arancio;
    }

    p {
        color: grey;
        font-size: 15px;
    }
}
</style>