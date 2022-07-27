<template>
  <section>
    <FeaturedArticles />
    <PostsList />
  </section>
</template>

<script>
import FeaturedArticles from './FeaturedArticles.vue';
import PostsList from './PostsList.vue';

export default {
  name: 'MainWeb',
  components: {
    FeaturedArticles,
    PostsList,
  }
}
</script>

<style lang="scss" scoped>

</style>