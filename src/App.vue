<script>
import { store } from './store'

import AppHeader from './components/AppHeader.vue';
import AppBarbers from './components/section/AppBarbers.vue';
import AppServices from './components/section/AppServices.vue';
import AppProducts from './components/section/AppProducts.vue';
import AppReviews from './components/section/AppReviews.vue';
import AppPosts from './components/section/AppPosts.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppBarbers,
    AppServices,
    AppProducts,
    AppReviews,
    AppPosts,
    AppFooter,


  },
  data() {
    return {
      store,
    }
  }
}




</script>

<template>
  <AppHeader />
  <main>
    <AppBarbers />
    <AppServices />
    <AppProducts />
    <AppReviews />
    <AppPosts />
  </main>

  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables.scss' as *;
@use './styles/partials/mixins.scss' as *;
</style>
