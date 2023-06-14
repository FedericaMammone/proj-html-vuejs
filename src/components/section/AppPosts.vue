<script>
import AppPostsCard from './AppPostsCard.vue'

export default {
    name: 'AppPosts',
    components: {
        AppPostsCard
    },

    data() {
        return {
            cards: [
                {
                    "image": '../../../public/avadabarbers-second-blog-320x202.jpg',
                    "title": 'Avada Barbers Now Open',
                    "description": 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt voluptatum nemo accusantium aspernatur incidunt nihil sequi dolor, quia, tempore  aperiam consectetur vero.'
                },
                {
                    "image": '../../../public/avadabarbers-choosing-blog-320x202.jpg',
                    "title": 'Choosing The Right Barber',
                    "description": 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt voluptatum nemo accusantium aspernatur incidunt nihil sequi dolor, quia, tempore aperiam consectetur vero.'
                },
                {
                    "image": '../../../public/avadabarbers-ourservice-blog-320x202.jpg',
                    "title": 'Quick Service Guide',
                    "description": 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt voluptatum nemo accusantium aspernatur incidunt nihil sequi dolor, quia, tempore aperiam consectetur vero.'
                },

            ]
        }
    },
}

</script>

<template>
    <section>
        <div class="triangle">
            <img src="../../../public/triangle.svg" alt="">
        </div>
        <div class="posts">
            <span>TALES FROM THE BARBER SHOP</span>
            <h1>Recent Blog Posts</h1>


            <div class="row">
                <AppPostsCard v-for="card in cards" :details="card" />

            </div>
            <button>READ MORE FROM OUR BLOG</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

section {
    background-color: $similBianco;

    .triangle {
        width: 100%;
        transform: rotate(180deg);


        img {
            width: 100%;

        }
    }

    .posts {
        @include my-display-flex-column($type: 'center');
        min-height: 800px;
        margin-top: 20px;

        span {
            color: $arancio;
        }

        h1 {
            color: $grigio;
        }


    }
}
</style>