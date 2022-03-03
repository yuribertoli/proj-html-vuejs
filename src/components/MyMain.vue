<template>
  <main>
      <MyJumbotron/>
      <ProBarbers/>
      <ServicesPart/>
      <GroomingProducts/>
      <ReviewsPart/>
      <RecentBlogPosts/>
  </main>
</template>

<script>
import MyJumbotron from "./partialsMain/MyJumbotron.vue";
import ProBarbers from "./partialsMain/ProBarbers.vue";
import ServicesPart from "./partialsMain/ServicesPart.vue";
import GroomingProducts from "./partialsMain/GroomingProducts.vue";
import ReviewsPart from "./partialsMain/ReviewsPart.vue";
import RecentBlogPosts from "./partialsMain/RecentBlogPosts.vue";

export default {
    name: "MyMain",

    components: {
        MyJumbotron,
        ProBarbers,
        ServicesPart,
        GroomingProducts,
        ReviewsPart,
        RecentBlogPosts
    }
}
</script>

<style lang="scss" scoped>

</style>