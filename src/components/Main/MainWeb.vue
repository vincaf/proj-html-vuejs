<template>
  <section>
    <FeaturedArticles />
    <PostsList />
    <ArticleCategories />
    <LatestArticles />
  </section>
</template>

<script>
import FeaturedArticles from './FeaturedArticles.vue';
import PostsList from './PostsList.vue';
import ArticleCategories from './ArticleCategories.vue';
import LatestArticles from './LatestArticles.vue';

export default {
  name: 'MainWeb',
  components: {
    FeaturedArticles,
    PostsList,
    ArticleCategories,
    LatestArticles,
  }
}
</script>

<style lang="scss" scoped>

</style>