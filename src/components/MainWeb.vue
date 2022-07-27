<template>
  <section>
    <FeaturedArticles />
    <PostsList />
    <ArticleCategories />
  </section>
</template>

<script>
import FeaturedArticles from './FeaturedArticles.vue';
import PostsList from './PostsList.vue';
import ArticleCategories from './ArticleCategories.vue';

export default {
  name: 'MainWeb',
  components: {
    FeaturedArticles,
    PostsList,
    ArticleCategories,
  }
}
</script>

<style lang="scss" scoped>

</style>